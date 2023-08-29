# Aerial-Image-Segmentation

## About the Dataset

The dataset used in this project is a subset of the Massachusetts Roads Dataset, which comprises aerial images of Massachusetts. The full dataset consists of 1171 images, and each image is 1500×1500 pixels in size, covering an area of 2.25 square kilometers. The dataset is available for download [here](https://www.cs.toronto.edu/~vmnih/data/).

## Methodology

By employing machine learning techniques, it constructs and trains a segmentation model to accurately identify road areas in the images. The project begins by loading a subset of the Massachusetts Roads Dataset, consisting of 200 aerial images and their corresponding road masks. Technical features include data augmentation for diverse training samples, a custom dataset class for effective data handling, and data loaders for organized batch processing. The model architecture is based on the UNet design, implemented using the segmentation_models_pytorch library, which predicts road segments from input images. It employs a hybrid loss function, combining Dice loss and binary cross-entropy loss, for model optimization. The code encompasses both training and validation procedures, along with checkpointing the best model based on validation loss. During inference, the trained model is utilized to generate road segment predictions for an example image, and the results are visually compared to the ground truth. Overall, this code showcases the end-to-end process of building a road segmentation model, including data preprocessing, model architecture, training, evaluation, and inference, thereby enabling the automatic identification of road segments in aerial images.








