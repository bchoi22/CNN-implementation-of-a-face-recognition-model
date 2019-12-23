# CNN-implementation-of-a-face-recognition-model

This is a simple face recognition model based upon a Keras implementation of CNN that was used to tell the difference between dogs and cats using relatively little data (1000 pictures of dogs and 1000 pictures of cats, specifically) to train the model. The website for the original model is: https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html. With some modifications to the original model, I then tested it against pre-processed facial data. The objective is to recognize an individual’s face by training the model using only the individual’s images in different scenarios using CNN. The model would then be tested against a sample population of image data of other peoples’ faces to test the reliability of the model. Using an appropriate loss function and normalized data, the model can somewhat accurately recognize the face it was trained on apart from all the other image data of other peoples’ faces.

This model uses even less data (only 530 images of former President George W. Bush due to limited data) to train and have it rule out any other faces tested against it. Using the keras.preprocessing.image package, the data was organized such that it allows the ImageDataGenerator method to access our acquired data. Train, Validation, and Test directories were created with 2 subdirectories each; one called “bush,” and the other called “other.” To recognize a particular individual’s face by training the model using only the individual’s images in different scenarios using CNN.

Data Set
The data set used was pre-processed data collected from www.cs.umass.edu/lfw/. Labeled Faces in the Wild (LFW)is a public benchmark for face verification. The website hosted a rich set of celebrity and political figure image data. The data in total was:
• 18,233 images (250 x 250-pixel data, .jpg files)
• 5,749 people
• 1,680 people with two or more images
George W. Bush had the greatest number of pictures of any one person in the database (530 pictures) and was an obvious choice to first test our hypothesis that CNN would be able to recognize a person’s face against a host of others.  Besides data from LFW, we also downloaded 20 randomized images from internet and saved them in to 250X250 pixel data as of test data for comparison between models.
