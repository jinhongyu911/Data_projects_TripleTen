Project_04 - Image Classification (Faces)

Project Description
The supermarket chain Good Seed would like to explore whether Data Science can help them adhere to alcohol laws by making sure they do not sell alcohol to people underage.
You are asked to conduct that evaluation, so as you set to work, keep the following in mind:
The shops are equipped with cameras in the checkout area which are triggered when a person is buying alcohol.
Computer vision methods can be used to determine age of a person from a photo. The task then is to build and evaluate a model for verifying people's age.
To start working on the task, you'll have a set of photographs of people with their ages indicated.

Taks Performed
1. Load necessary packages and image, label datasets
2. EDA
* Check mean, median, and mode of the labels (ages)
* Sample and visualize the image dataset to check image sizes and image types
* Create train and test datagen flows, setting target size and batch size
3. Train CNN Model
* Create a ResNet50 CNN model adding pooling, dropout and flattened layers
* Compile the model using Adam optimizer
* Fit the model to the image dataset to train
* Evaluate the final model performance after 20 epochs

Conclusions
1. The model underwent a total of 20 epochs of training, with each epoch completing in 35 seconds on a GPU platform, indicating efficient processing.
2. Although the train_loss steadily decreased throughout the epochs, the val_loss began to plateau and even increase after the 10th epoch.
   This divergence suggests that the model started to overfit the training data.
3. To address this overfitting, it's advisable to either reduce the number of epochs during training or implement early stopping techniques to prevent the model from memorizing the training data.
4. The primary objective of this project is to develop a model capable of accurately verifying individuals' ages to prevent the sale of alcohol to minors.
   However, based on the observed train_mae and val_mae, it appears that the model's accuracy may not be sufficient to reliably achieve this goal.
5. Given the limitations in accuracy, it may be necessary to train a different model capable of achieving a lower MAE to mitigate the risk of unintentionally selling alcohol to minors.
6. Alternatively, a classification model could be developed to categorize individuals into three age groups: [<10], [10-30], and [>30].
   In cases where a customer falls into the middle category, their age could be verified by a human evaluator using their ID card.  
7. Conversely, a revised project objective could focus on implementing a model for scanning and detecting the date of birth on individuals' ID cards as a means of accurately determining their age.
   This approach could provide a more reliable means of age verification, potentially enhancing the effectiveness of the model in real-world scenarios.
