# Automatic Number Plate Detection 🚗

In this project, we have created an Automatic Number Plate Recognition system using `TensorFlow Object Detection`. This will take as input images of vehicles with number plates along with its annotations. Annotations contain information about the location of number plate on an image in the form of `xmin`, `ymin`, `xmax`, `ymax`. We need this specific tag from the XML annotations file in order for the mode to train on the images and learn to detect number plates.

The dataset used to train the model is from `Kaggle`, which already has images annotated and saved in the form of an `.xml` file. So we don't have to manually annotate images. 

⏩ Link to the Dataset: https://www.kaggle.com/datasets/andrewmvd/car-plate-detection

⚠🧯 Just a word of caution. If and only if you have a powerful GPU, then only run it on your local machine and if case if you don't, run it on google colab, that's where I ran my notebook.

