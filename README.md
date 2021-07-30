# Realistic-Face-Image-Generator
This project uses the concept of GAN's to create a Generator-Discriminator model that work on creating realistic looking human faces, with the training dataset being from the CelebA dataset.
# Dataset
The dataset used - https://s3.amazonaws.com/video.udacity-data.com/topher/2018/November/5be7eb6f_processed-celeba-small/processed-celeba-small.zip

It is made up of celebrity faces that are mostly white, but is definitely more complex than datasets like MNIST and SVHN
# Model
The model consists of a :-
Generator - Takes random noise as input and produces fake images of size 32x32x3. We have used 4 convolutional layers with batch normalization in all layers except first one. ReLU activation function is used in first 3 layers and tanh acivation is used in the last layer.

Discriminator - Main role is to distinguish between fake and real images. Takes a 32x32x3 image and gives output as real or fake. Our model has no maxpooling layers and is also using 4 convolutional layers with batch normalization except the first layer. Activation function used is Leaky ReLU.
# Output

<img width="720" alt="op1" src="https://user-images.githubusercontent.com/60126229/127672670-9c714544-aae9-4b1e-a47b-8643d78e966e.PNG">

<img width="723" alt="op2" src="https://user-images.githubusercontent.com/60126229/127672711-ffeaa596-64fb-4314-85ea-700e96b637c2.PNG">


