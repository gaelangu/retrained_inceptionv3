# Facial Recognition using Pre-trained Inception v3


This is based on the Tensorflow for Poets codelab, which can be found [here](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets). The model was originally used to classify types of flowers.

The final softmax-classifier layer of the Inception model has been retrained on:

* 133 images of the *host*; photos of myself from Facebook and multiple extracted video frames
* 345 images of the *guest*; various pictures of Lee Hsien Loong taken from Google using the Fatkun Batch Download Image tool


To classify new images, key in the Terminal:

`python label_image.py gg1.jpg`

Classification scores of both *host* and *guest* will be output. Classification scores for *host* tend to be better when only the face of the *host* is captured in the frame - that is one limitation of the current retrained model.


To retrain on new images, follow the Tensorflow for Poets codelab step [here](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/#7).
