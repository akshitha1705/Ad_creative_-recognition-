# Ad_creative_recognition
In today's fast-paced digital world, advertisements are crucial for capturing attention and engaging users. However, distinguishing between ad creatives and regular images poses a significant challenge. The goal of this project is to develop an intelligent solution that can accurately identify ad creatives, enhancing the efficiency and effectiveness of digital advertising.
# Dataset
The dataset consists of approximately 4700 advertising images and 650 non-advertising images collected from various sources.
# Data Preprocessing
To ensure consistency in size, format, and quality, and to prepare the data for training, several preprocessing techniques were applied such as Resizing,Normalization,Data Augmentation Techniques such as flipping, rotating, and applying Gaussian blur are applied to increase the variability of the training set and prevent overfitting.
# Model Architecture
The VGG16 model is chosen as the backbone of the image classification task. VGG16, developed by the Visual Geometry Group at the University of Oxford, is renowned for its simplicity and effectiveness. It uses a stack of convolutional layers with small receptive fields (3x3) and is followed by max-pooling layers.
- The **Flatten** layer converts the 3D feature maps to 1D feature vectors.
- The **Dense** layer with 512 units and ReLU activation learns complex patterns from the features.
- The **Dropout** layer helps in preventing overfitting by randomly setting a fraction of input units to 0 at each update during training.
- The final **Dense** layer with sigmoid activation outputs the probability of the image being an ad creative.
# Training
The model is trained on the training data and saved the model weights for future use.
# Evaluation
The model is evaluated on the test data to measure its performance. The model achieved approximately 97% accuracy and a 0.97 F1 score, indicating its effectiveness in recognizing ad creatives with minimal false positives.
# Classification
The classification model predicts whether an image is an advertising creative or a non-advertising image, enhancing the efficiency and effectiveness of digital advertising by automating the identification process.
