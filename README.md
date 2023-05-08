# Emotion AI
Artificial Emotional Intelligence or Emotion AI is a branch of AI that allows computers to understand human non -verbal cues such as body language and facial expressions.
### PROJECT OVERVIEW
The aim of this project is to classify people’s emotions based on their face images. <br>
 - In this project, we will work as on AI/ML. <br> 
 - We will train and deploy a system that automatically monitors people's emotions and expressions. <br>
 - We have collected more than 20000 facial images, with their associated facial expression labels and around 2000 images with their facial key-point annotations. <br>
<br><br>![Screenshot 2023-05-08 200906](https://user-images.githubusercontent.com/98466525/236865471-4e3d7704-9701-476f-8ca2-69969d1efb2b.png)
### Part 1 : KEY FACIAL POINTS DETECTION
In part 1, we will create a deep learning model based on Convolutional Neural Network and Residual Blocks to predict facial key-points.
The dataset consists of x and y coordinates of 15 facial key points.
 - Input Images are 96 x 96 pixels.
 - Images consist of only one color channel (gray-scale images). <br> 
<br>

### Part 2 :  FACIAL EXPRESSION (EMOTION) DETECTION

The second model will classify people’s emotions. <br> 


Data contains images that belong to 5 categories:

 - 0 = Angry
 - 1 = Disgust 
 - 2 = Sad 
 - 3 = Happy 
 - 4 = Surprise

In this we use the neural network with the architecture given below to predict the emotion Class of emotion described above.In this model get the image in the form of a pixel as the input and and then the prediction in the form of emotion. The emotion which has the highest probability is 1 and all others are zero. 
<br><br> ![Screenshot 2023-05-08 201118 hehe](https://user-images.githubusercontent.com/98466525/236868708-b272d3bd-1a1a-47a4-9e3e-77dee671e17c.png)

#### RESNET (RESIDUAL NETWORK):
 - As CNNs grow deeper, vanishing gradients tend to occur which negatively impact network performance. 
 - Vanishing gradient problem occurs when the gradient is back -propagated to earlier layers which results in a very small gradient. 
 - Residual Neural Network includes a “skip connection” feature which enables training of 152 layers without vanishing gradient issues. 
 - Resnet works by adding “identity mappings” on top of CNN. 
 
<br><br> ![Screenshot 2023-05-08 201237h](https://user-images.githubusercontent.com/98466525/236869165-c5cfbfa3-415b-498e-8ace-be1db7a3fb22.png)
<br><br> ![Screenshot 2023-05-08 201255h1](https://user-images.githubusercontent.com/98466525/236869288-a0c5b45c-1535-46fb-ad81-a92c91f8a781.png)

#### Combining the both model:
In the end we combine the both models. After training the model we give the model the testing data which is in the form of pixels and the first part gives the key facial point and the second part gives the emotion prediction for this.

<br><br> ![Screenshot 2023-05-08 201432h2](https://user-images.githubusercontent.com/98466525/236869600-07c68891-0502-43f5-9368-7f2a72b89a87.png)


