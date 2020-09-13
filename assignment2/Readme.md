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
    
  * Batch Normalization
    * Datasets:CIFAR10 
    * Experiment process: We strategy is to change the architecture of the network to make it easier to train,we will use Batch Normalization and Layer Normalization.
    * Experiment result:   
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/BatchNormalization_result.png)  
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment2/pic2/BatchNormalization_result.png)  
    As shown in the figure above,we can find that we can get better accuracy using BN in different batch size. 

 
 * Dropout
    * Datasets:CIFAR10 
    * Experiment process: 
    * Experiment result:   

 * Convolutional Networks
    * Datasets:CIFAR10 
    * Experiment process: We develop a neural network with fully-connected layers to perform classification,and we tune our hyperparameters.
    * Experiment result: Best Validation accuracy: 0.509000 h_size: 125 learning rate: 0.001100 reg: 0.750000  
      we visualize the learned weights for each class  
      ![](https://github.com/fanshuhuangjia/cs231n/blob/master/PIC/tow_layer_net_learned%20weights.png)
 * PyTorch on CIFAR-10
