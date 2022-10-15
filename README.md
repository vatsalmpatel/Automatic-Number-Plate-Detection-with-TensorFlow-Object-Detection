# Automatic Number Plate Detection 🚗

In this project, we have created an Automatic Number Plate Recognition system using `TensorFlow Object Detection`. This will take as input images of vehicles with number plates along with its annotations. Annotations contain information about the location of number plate on an image in the form of `xmin`, `ymin`, `xmax`, `ymax`. We need this specific tag from the XML annotations file in order for the mode to train on the images and learn to detect number plates.

The dataset used to train the model is from `Kaggle`, which already has images annotated and saved in the form of an `.xml` file. So we don't have to manually annotate images. 

⏩ Link to the Dataset: https://www.kaggle.com/datasets/andrewmvd/car-plate-detection

⚠🧯 Just a word of caution. If and only if you have a powerful GPU, then only run it on your local machine and if case if you don't, run it on google colab, that's where I ran my notebook.

# How to run the notebook❓

If I were you, what I would do is copy this entire notebook to Google Colab and run it cell by cell from the very top to the very bottom and just study the code to see what each line is doing and if you encounter some errors, `Google` them.

## Some errors that you are going to run into 😭

▶ When you get to the setp of generating `TFRecords` for training and testing, you will need to change some code in the `generate_tfrecords.py` file. From line `88`, you will find these 4 lines ⬇, originally, the code would have 4's instead of all 5's, you need to change these to all 5's, and the reason for this is because in the annotations file, the actual `bounding box` coordinates are at position 5, not 4.

```Python
int(member[5][0].text),
                     int(member[5][1].text),
                     int(member[5][2].text),
                     int(member[5][3].text)
```

### Apart from these, the code is straight forward, the code script takes care of everything for you, and if any errors occurs, just `Google` and see if you can find a solution for it (probably you will). Enjoy ✅🏁.