# RoadDetectionUsingYoloV2
A jupyter notebook showing Object detection for custom models, the algorithm i trained was to detected roads from aerial photos 


This is a example of a object detection using darknet and yoloV2.

The model was trained on google collaboratory using the tesla GPU

The model used is based on the tiny yolo model for 1 class which is roads

For preparing my training dataset i got many images of aerial view of roads and cities , and annotated the roads using the software labelImg

This model was trained for 10 thousand steps, each taking around 1 second

The directory structure to replicate this experiment must be as follows:

notebook
darknet folder
Arquitetura
Dados
testdata



and inside these folders


darknet folder

The instalation of darknet, with GPU set to 1 on Makefile, the notebook shall run it

Arquitetura:
cfg model file
obj.data contains the number of classes path to training and testing file as well as weights backup path
obj.names contains the names of each class on the training set



Dados:

Contains training and validation images as well as their txt files with yolo expected format

Also contains the train and test files which contains the absolute path of the images used for training and validation

testdata:

Contains a set of images not used in the training process, these will be used to validate how the model handles unseen data
