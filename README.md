# cs231n

  Assignment #1: Image Classification, kNN, SVM, Softmax, Fully-Connected Neural Network  
  Assignment #2: Fully-Connected Nets, BatchNorm, Dropout, ConvNets, Tensorflow/Pytorch  
  Assignment #3: Image Captioning with Vanilla RNNs and LSTMs, Neural Net Visualization, Style Transfer, Generative Adversarial Networks  
# Assignment 1  
  * k-Nearest Neighbor classifier  
    * Datasets:CIFAR10 
    * Experiment process: We build a KNN model to classify the data,and then we change the value of k.We try to determine the best value of this hyperparameter with cross-validation.
    * Experiment result:   
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/PIC/knn_result.png)  
    At last,we use k = 10,and get 144 / 500 correct => accuracy: 0.288000
  * Support Vector Machine
    * Datasets:CIFAR10 
    * Experiment process: We build a SVM model to classify the data.And we use the validation set to tune hyperparameters(learning_rates = [1e-7, 5e-5],regularization_strengths = [2.5e4, 5e4]).
    * Experiment result: We visualize the cross-validation results as follows:  
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/PIC/SVM_hyperpaprameters.png)  
    At last,we get a accuracy: 0.375000,and we visualize the learned weights for each class  
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/PIC/SVM_learned%20weights.png)  
  * Softmax classifier
    * Datasets:CIFAR10 
    * Experiment process: We build a Softmax classifiler to classify the data.And we use the validation set to tune hyperparameters(learning_rates = [1e-7, 5e-7],regularization_strengths = [2.5e4, 5e4]).
    * Experiment result: softmax on raw pixels final test set accuracy: 0.360000(learning_rates=5e-7,regularization_strengths=2.5e4)  
      we visualize the learned weights for each class  
    ![](https://github.com/fanshuhuangjia/cs231n/blob/master/PIC/Softmax_learned%20weights.png)
  * Two-Layer Neural Network
    * Datasets:CIFAR10 
    * Experiment process: We develop a neural network with fully-connected layers to perform classification,and we tune our hyperparameters.
    * Experiment result: Best Validation accuracy: 0.509000 h_size: 125 learning rate: 0.001100 reg: 0.750000  
      we visualize the learned weights for each class  
      ![](https://github.com/fanshuhuangjia/cs231n/blob/master/PIC/tow_layer_net_learned%20weights.png)
  * Image Features(not finished)
