# Birds_classification

Dataset is used from [Kaggle](https://www.kaggle.com/datasets/gpiosenka/100-bird-species).

Data set of 400 bird species. 58388 training images, 2000 test images and 2000 validation images. This is a very high quality dataset where there is only one bird in each image and the bird typically takes up at least 50% of the pixels in the image. As a result even a moderatly complex model will achieve training and test accuracies in the mid 90% range. All images are 224 X 224 X 3 color images in jpg format. 

To run this notebook on colab first upload your Kaggle API Json in colab to download data.

Dataset is loaded using Keras [Image Dataset Utility](https://www.tensorflow.org/api_docs/python/tf/keras/utils/image_dataset_from_directory).

1. 3 Layer CNN model was trained.
    - Train Accuracy : 97.7%
    - Validation accuracy: 54.85%
2. 3 Layer CNN model with Data Augmentation and Dropout Layer.
    - Train Accuracy : 61.75%
    - Validation accuracy: 65.955%
3. Transfer Learning with Pretrained EfficientNetB7.
    - Train Accuracy : 96.68%
    - Validation accuracy: 90.0%
4. Transfer Learning with Pretrained EfficientNetB2 and Data Augmentation.
    - Train Accuracy : 94.91%
    - Validation accuracy: 93.20%
    
## References
[Image classification](https://www.tensorflow.org/tutorials/images/classification)

[Transfer learning and fine-tuning](https://www.tensorflow.org/tutorials/images/transfer_learning)

[Load and preprocess images ](https://www.tensorflow.org/tutorials/load_data/images)
