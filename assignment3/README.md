# Assignment 3  
  * Image Captioning with Vanilla RNNs  
    * Data sets:MS-COCO  
    For this exercise we will use the 2014 release of the Microsoft COCO dataset which has become the standard testbed for image captioning. The dataset consists of 80,000 training images and 40,000 validation images, each annotated with 5 captions written by workers on Amazon Mechanical Turk.To cut down on processing time and memory requirements, we have reduced the dimensionality of the features from 4096 to 512
    * Evaluation Metrics: None
    * Compared Methods: None
    * Experimental Setup: 
      Ubuntu16.04   
      requirements:listed in the requirements.txt  
      batch size: 25  
      epoch: 50  
      train size: 100  
      val size: 2  
    * Qualitative Results:  
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/RNN_caption_train.png)
                           ![](https://github.com/fanshuhuangjia/cs231n/blob/master/assignment3/pic/RNN_caption_val.png)
    * Further Discussion: The samples on training data should be very good; the samples on validation data probably won't make sense.



