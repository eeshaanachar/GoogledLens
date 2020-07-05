# Googled Lens
Googled lens is an optical character recognition system inspired by Google Lens.

### Objective(s)
* To identify text from images.

### Platform
Googled Lens is developed with Python, mainly with the Keras and OpenCV libraries. The code is loaded onto a .ipynb file for an interactive interface.

### Working Principle
Individual characters are identified based on the contrast between the foreground and the background of the image. These characters are then fed into a convolutional neural network model, trained with data from the emnist dataset, to perform the predictions. The results are then written on the image on the upper left corner of the corresponding identified character.

### Present Scope
* Characters must be well separated (cursive handwriting will completely fail).
* No GUI. A mobile app with which images can be clicked would be ideal.
* Poor noise handling capability.
* A small but significant number of misclassifications are present. A second layer to rectify misclassifications using context could be added.
* The parameters of each image must be manually adjusted.
* The text needs to be of dark color on a light background. A sliding window technique for classifying texts would be good.