# Assignment 3  
  * Image Captioning with Vanilla RNNs  
    * Data sets:MS-COCO  
    For this exercise we will use the 2014 release of the Microsoft COCO dataset which has become the standard testbed for image captioning. The dataset consists of 80,000 training images and 40,000 validation images, each annotated with 5 captions written by workers on Amazon Mechanical Turk.To cut down on processing time and memory requirements, we have reduced the dimensionality of the features from 4096 to 512
    * Experimental Setup: 
      Ubuntu16.04   
      requirements:listed in the requirements.txt  
      batch size: 25  
      epoch: 50  
      train size: 100  
      val size: 2  
    * Qualitative Results:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/RNN_Caption_train.png)
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/RNN_Caption_val.png)
    * Further Discussion: The samples on training data should be very good; the samples on validation data probably won't make sense.

  * Image Captioning with LSTMs  
    * Data sets:MS-COCO  
    For this exercise we will use the 2014 release of the Microsoft COCO dataset which has become the standard testbed for image captioning. The dataset consists of 80,000 training images and 40,000 validation images, each annotated with 5 captions written by workers on Amazon Mechanical Turk.To cut down on processing time and memory requirements, we have reduced the dimensionality of the features from 4096 to 512
    * Experimental Setup: 
      Ubuntu16.04   
      requirements:listed in the requirements.txt  
      batch size: 25  
      epoch: 50  
      train size: 100  
      val size: 2  
    * Qualitative Results:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/LSTM_Caption_train.png)
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/LSTM_Caption_val.png)
    * Further Discussion: The samples on training data are very good; the samples on validation data still don't make sense.(because of overfitting)


  * Network Visualization: Saliency maps, Class Visualization, and Fooling Images  
    * Data sets:ImageNet
    We have provided a few example images from the validation set of the ImageNet ILSVRC 2012 Classification dataset.Since they come from the validation set, our pretrained model did not see these images during training.
    * Experimental Setup: 
      Ubuntu16.04   
      requirements:listed in the requirements.txt  
      pre_trained model: SqueezeNet
    * Qualitative Results:  
                           Saliency Maps:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/NV_Saliency_maps.png)  
                           Fooling Images:
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/NV_Fooling_images.png)  
                           Class Visualization:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/NV_Class_visualization.png) 

     
  * Style Transfer
    * Data sets:  five pictures(composition_vii,muse,starry_night,the_scream,tubingen)
    * Experimental Setup: 
      Ubuntu16.04   
      requirements:listed in the requirements.txt  
      pre_trained model: SqueezeNet
    * Qualitative Results:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/StyleTransfer1.png)
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/StyleTransfer2.png)
    
  * Generative Adversarial Networks  
    * Data sets:Pytorch MNIST  
    For this exercise we will use MNIST as our dataset.The default parameters will take 5,000 of the training examples(50000) and place them into a validation dataset
    * Experimental Setup: 
      Ubuntu16.04   
      requirements:listed in the requirements.txt  
      batch size: 128  
      epoch: 10  
      train size: 50000  
      val size: 5000  
    * Qualitative Results:  
                           Vanilla GAN:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/Vanilla_GAN.png)  
                           LS-GAN:
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/LS_GAN.png)  
                           DC-GAN:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/DC_GAN.png) 
    * Further Discussion: The Vanilla GAN use Fully connected layer in the Discriminator and Generator,but the result was not good. The LS-GAN proposed a newer, more stable alernative to the original GAN loss function,and got a bit improvement.The DC-GAN used convolutional network instead of fully connected network and got a better results.

