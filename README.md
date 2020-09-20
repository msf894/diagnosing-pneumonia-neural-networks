# Introduction:

The computing power of neural networks is one that has harnessed into a vast number of fields and industries. Due to their ability to detect complex patterns and learning how to improve their accuracy, it has been especially effective in the realm of image classification. The medical field has been especially invested in using neural networks for diagnosing patients from medical scans for accuracy and faster turnaround times. The purpose of this project was to develop a neural network that is capable of identifying pneumonia from chest x-rays of patients. Over the course of this project, I reiterated through several designs and architectures attempting to improve overall accuracy and recall for detecting pneumonia.

![xray images](/images/xray_images.png)

# Data Information:

The dataset used consisted of nearly 6,000 chest x-rays of pediatric patients from the from Guangzhou Women and Children’s Medical Center. The images have already been pre-classified as whether the patient had pneumonia or not. These images were already pre-split into different folders for testing, training, and validation. The dataset provided was taken from Kaggle at the following link: https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

# Models and Results:

I initially developed multiple convolutional neural networks(CNNs) with different architectures as a baseline measurement for performance. CNNs have been especially used for image classification due to their ability to detect and learn complex patterns within image regions. I also used several pretrained neural networks, specifically VGG19 and Xception. These pretrained models have already been trained on datasets consisting of millions of images and can act as a general model that can be applied for various problems

The primary metrics used for evaluating the models were overall accuracy and recall for pneumonia patients. I wanted to develop a model that would not only perform well overall but one that was particularly effective at diagnosing pneumonia correctly. A patient with pneumonia that is incorrectly diagnosed as healthy could suffer serious complications, especially the high risk infants and children from which we have these images from.

![neural network results](/images/Neural_Network_Results.png)

Out of all the models tested, Xception performed the best in terms of overall accuracy and recall. Xception achieved an 88% overall accuracy and 83% recall on patients with pneumonia.

![Xception_Results](/images/Xception_Results.png)

# Conclusion:

Pre-trained neural networks seemed to have the best performance of all the models tested, specifically Xception. For future projects, I'd like to look into implementing neural networks for diagnosing other illnesses that can be detected though medical scans, such as cancer or COVID-19. I'd also like to explore other and larger datasets for x-rays in the hopes of creating a specialized neural network specifically for x-rays to detect anomalies. Lastly, I want to see if this technology performs well with other mediums of medical imaging such as CT and MRI scans.
