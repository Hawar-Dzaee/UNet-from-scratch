# U-Net Image Segmentation for Multi-Class Object Labeling

This project demonstrates the implementation of a U-Net architecture from scratch for multi-class image segmentation. The U-Net model is designed to label objects in images such as roads, cars, pedestrians, and other urban features, across 12 different classes. The architecture is inspired by the paper "U-Net: Convolutional Networks for Biomedical Image Segmentation" and has been adapted for the task of labeling urban environments.



## Key Components

### 1. U-Net Architecture
The U-Net architecture is known for its excellent performance in image segmentation tasks, particularly in biomedical fields. In this project, we have adapted the U-Net model for urban segmentation, targeting various objects within urban environments. We utilize VGG16 as the backbone for the encoder, enhancing the model's feature extraction capabilities and improving the overall segmentation performance, especially for complex urban landscapes.

![U-Net](https://github.com/user-attachments/assets/7e7ab8cc-b87f-4602-8d8a-f5a79564c519)

The original research paper can be accessed here: [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597).

### 2. Multi-Class Segmentation
We apply U-Net for a multi-class segmentation problem, labeling various urban objects. Each pixel in the image is assigned a class from the following list:

Road
Car
Pedestrian
Building
Tree
Other relevant urban classes (total of 12 classes)

<img width="791" alt="Screen Shot 2024-09-13 at 12 01 24 PM" src="https://github.com/user-attachments/assets/d174b214-aab0-40e1-b7a6-b7628486b777">


### 3. Model Training
During training, the model’s performance is tracked using Neptun.ai for experiment management and Plotly for interactive visualizations.
Neptun.ai: Track the learning curves, model metrics, and hyperparameters using Neptun.ai. It provides interactive visualizations and insights into the training process.
Plotly Figures: Learning curves (accuracy, loss) and other metrics are visualized using Plotly. These figures help in understanding model performance over time.

### 4. Dataset
The dataset used for training and evaluation consists of images from urban environments, where each image is labeled with 12 different object classes. Preprocessing steps include resizing the images, normalizing pixel values, and applying data augmentations such as flipping, rotation, and scaling.

### 5. Model Evaluation
The model is evaluated using metrics Cross Entropy Loss.


## Results
During model training, learning curves (accuracy, loss) are plotted using Plotly. Examples of these learning curves can be found in the results section of the notebook.
Neptun.ai Integration: You can view interactive metrics and model performance via Neptun.ai. It provides detailed tracking of training metrics, which helps in fine-tuning the model.

![plotly](https://github.com/user-attachments/assets/97ebec40-6145-4063-9ad4-ee22f52c4fe4)


## Future Work
Implement more advanced data augmentation techniques.
Fine-tune the model on larger datasets for improved performance.
Experiment with other segmentation architectures (e.g., DeepLabV3, Mask R-CNN).







