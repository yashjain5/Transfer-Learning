# Transfer Learning
In transfer learning, a base network is trained on a base dataset and then the learned features are transferred to a second target network which is to be trained on a target dataset. This process works if the features are general to both base and target tasks, instead of being specific to the base task. 

Generally, two approaches are followed to implement transfer learning - develop model approach and pre-trained model approach. In this project we will implement the pre-trained model approach, where we use a pre-trained base model as the starting point for training a target network.

# Project Description
In this project, we leverage a RetinaNet50 architecture pre-trained classifier for its feature extraction capabilities and then re-train it on a small set of images to create a tight bounding box around the new object. We will use Google Colab for training our model and Google Drive for storing the output results.

# Aim
1)	To collect 5 images of a rubber duck and then manually annotate them.
2)	Loading the SSD ResNet50 (RetinaNet50) pre-trained model and then fine-tuning it on the above collected images. 
3)	Running the object detection algorithm on a new image to identify the rubber duck.
4)	Making a gif using imageio after applying the model to the test images.

# Running the code on Google Colaboratory
The project requires you to mount your Google Drive to the location /content/gdrive in Google Colab. There are a few initial steps to follow before executing the code.
First, you need to make a new folder in your Google Drive by the name “transfer_learning_project” [without double quotes].

Now in model.ipynb notebook,
1)	Go to Runtime &#8594; Change runtime type &#8594; Set the hardware accelerator as GPU

2)	Run the first cell of the notebook in colab shell. You will be given a URL and you will be asked to enter an authentication code to mount your Google Drive. 

After following the above steps, you can run the other cells in sequence and the final outputs will be saved in the ‘transfer_learning_project/results’ folder in your Google Drive account.

# Results 
![rubber_duck_detection.gif]( results/rubber_duck_detection.gif)

