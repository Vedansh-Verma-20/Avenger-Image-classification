# Avenger-Image-classification
Classifies  an Avenger character's image into one of 5 classes
 Problem Statement-1)Create a labeled dataset of Avengers images- Captain America, Iron Man,Black Widow, Hulk,Spider Man (exchanged thor with spider man)
                   2)Then Train a CNN that is able to classify an unseen image
                   
 Approach:
 
    1)To make the dataset i downloaded marver heros dataset from kaggle link- https://www.kaggle.com/datasets/hchen13/marvel-heroes
      This dataset has train and valid subfolders, in each of which there are 8 classes-black widow,captain america, doctor strange, hulk, iron man, loki, spider-man    and       thanos.
      Train folder had - 400 images of each classes 
      Valid folder had- 55 classes
      In order to reduce the no. of image and classes, I deleted the image folder of loki, doctor strange and thanos from both train and valid folders, giving me       remaining 5 classes,  after  which for train folder I reduced no. of images in each class to around 300 and didn't change anything in valid class.
     2) Made a new avenger photo folder from  my earlier step, then uploaded its zip format to Google Colab
     3) Unzipped the folder thrhough code, this will now reprsent my data
     4)Imported all libraries
     5)Specified the transform needed to be done on input image
     6) constructed dataset for traina and valid usind data available on colab space
     7)Defined  training model
     8) downloaded the VGG16 convolutional network which is well known CNN model
     9) freezed its all layers for training
     10) defined extra linear layer to be trained 
     11)Specified optimizer and loss fuction to use
     12) trainied the model for 5 epochs
Tools used: Pytorch, google colab     
 
