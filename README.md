#### Sign Language Alphabet Recognition
This GitHub repository contains an American Sign Language (ASL) alphabet detector. The detector uses mediapipe and opencv to recognize and classify hand gestures representing the 26 letters of the ASL alphabet. The model was trained on a dataset of images of hand gestures and the corresponding ASL letters. The code provide an end-to-end solution for anyone interested in developing a similar project, from data preprocessing to model training and evaluation.

![](asl.png)

#### Requirements:
* [NumPy](http://www.numpy.org/)
* [OpenCV](https://docs.opencv.org/4.x/)
* [Scikit-Learn](https://scikit-learn.org/stable/getting_started.html)
* [MediaPipe](https://mediapipe.dev/)

#### Datasets i used:
[Synthetic ASL Alphabet - Kaggle](https://www.kaggle.com/datasets/lexset/synthetic-asl-alphabet) <br />
[American Sign Language Letters Dataset - RoboFlow](https://public.roboflow.com/object-detection/american-sign-language-letters)

#### Example:
![](example_image.png)

<hr>

The model had a ~98% accuracy on the test set (who came from the same distribution as the train set), although when i used the model on new images a few problems came out:

- the letter 'S' was usually mistaken with the letter 'N'
- the letter 'J' requires hand movement and since the model was trained only on static images it is often mistaken with 'I'
