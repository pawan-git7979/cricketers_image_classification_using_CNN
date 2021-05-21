# cricketers_image_classification_using_CNN
Build a image classfication CNN  in deep learning using Keras and Tenserflow2.0 , of indian cricketers. 

![Image_Classfication_Model_Using_CNN](https://user-images.githubusercontent.com/63632573/119144837-b15c9f80-ba66-11eb-9629-da60e918123f.png)

In this Project I have tried to build a CNN model for the image classfication which is classifying the images of the Indian Cricketers.
Their are around 576 images available, which belongs to 15 class labels.

To build this model I have used various techniques and approaches.
- Build simple CNN
- Build CNN and applied data augmentation
- Build CNN using keras_Tuner technique
- Transfer Learning

Let's Talk about one by one 
### <u>simple CNN</u>
In simple CNN model, I have toal of 576 images of different-different indian cricketers. 
I have used the validation split of 0.2.
- train data = 80%
- test data  = 20%

The accuracy of my model is-
- train data = 99%
- test data = 43%

### CNN using Data Augmentation
Data Augmentation is a very popular technique in the deep learning, which is used to transform the images by different different properties 
like zoom in, horizontal flip, reversing etc.
Data Augmentation helps us to make the model more **robust** and helps to us to generate more data upn which model can be trained.
 

- train data = 80% (around 462 images)
- test data  = 20% (around 114 images)

The accuracy of the model is-
- train data = 91%
- test data = 37%

### CNN using keras_Tuner
Keras_tuner is a hyperparameter tuning technique which is used in your model to find the best hyperparameters like no of filters, filter size,
no of conv2D layer etc.

For using keras_Tuner, you can dowunload it by running
> !pip install keras-tuner

 - train data = 80% (around 462 images)
 - test data  = 20% (around 114 images)


The accuracy of the model is-
- train data = 90%
- test data = 42%

### Transfer Learning
In transfer learning is a technique in which we used the pre-trained model, which is already ha been trained on thousands of images.
To use this in our model, we just have to delete the last layer of the model and have to append our layer.

Inside the transfer learning, I have used **VGG16** model which is the best model for the image classfication.

 - train data = 80% (around 462 images)
 - test data  = 20% (around 114 images)

Accuracy of the model is

![Screenshot from 2021-05-21 14-04-52](https://user-images.githubusercontent.com/63632573/119150186-d4d61900-ba6b-11eb-9047-8e6d1d033cf9.png)

- train data = 90%
- test data = 53%

Loss data


![Screenshot from 2021-05-21 14-06-02](https://user-images.githubusercontent.com/63632573/119150088-be2fc200-ba6b-11eb-8241-b97eb2bd8ca1.png)



## The accuracy by using the Transfer Learning technique and VGG16 model is highest among all of these. But this can still be improved a lot.


 

