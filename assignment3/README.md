# Assignment 2  
  * Fully-connected Neural Network  
    * Datasets:CIFAR10 
    * Experiment process: In this exercise we will implement fully-connected networks using a more modular approach. In addition to implementing fully-connected networks of arbitrary depth, we will also explore different update rules for optimization, and introduce Dropout as a regularizer and Batch/Layer Normalization as a tool to more efficiently optimize deep networks.
    * Experiment result:  So far we have used vanilla stochastic gradient descent (SGD) as our update rule. More sophisticated update rules can make it easier to train deep networks. We will implement a few of the most commonly used update rules and compare them to vanilla SGD.  
    SGD+Momentum: Add a 'momentum' to our gradient so that we can avoid being trapped in saddle point.  
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/SGD-Momentum.png)  
    And we got a better lost and accuracy when we use SGD+Momentum:  
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/SGD-result.png)  
    RMSProp and Adam:This method is beneficial to eliminate the direction of large swing amplitude, and is used to modify the swing amplitude, so that the swing amplitude of each dimension is smaller.  
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/RMSProp.png)  
    Adam:Combine the advangetage of Momentum and RMSProp  
    We have showed the results as following:
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/RMS_Adam.png)  
    As shown in the figure above,we got better lost and accuracy when we use RMSProp and Adam.Because of combining the advangetage of Momentum and RMSProp,Adam got the best performance in our experiments.
    
  * Batch Normalization
    * Datasets:CIFAR10 
    * Experiment process: We strategy is to change the architecture of the network to make it easier to train,we will use Batch Normalization and Layer Normalization.  
                          ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/BN.png) 
    * Experiment result:   
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/BatchNormalization_result.png) 
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/Layer%20Normalization_result.png)
    As shown in the figure above,we can find that we can get better accuracy using BN and LN in different batch size. 

 
 * Dropout
    * Datasets:CIFAR10 
    * Experiment process: Dropout is a technique for regularizing neural networks by randomly setting some output activations to zero during the forward pass.  
                          ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/dropout.png)  
                          As an experiment, we will train a pair of two-layer networks on 500 training examples: one will use no dropout, and one will use a keep probability of 0.25. We will then visualize the training and validation accuracies of the two networks over time.  
    * Experiment result:   ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/dropout_result.png)  
                           As shown in the figure above,we can find that using dropout will lower train accuracy,but improve val accuracy. 

 * Convolutional Networks
    * Datasets:CIFAR10 
    * Experiment process:  We build a three-layer convolutional network with the following architecture:  
                           conv - relu - 2x2 max pool - affine - relu - affine - softmax
    * Experiment result:  At last we got full data training accuracy 0.49 and full data validation accuracy: 0.483 in the CIFAR10   
                          We visualize the first-layer convolutional filters from the trained network.  
                          ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/CNN_result.png) 
