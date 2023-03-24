Generative Adversarial Networks (GAN) Project

This project aims to create a Generative Adversarial Network (GAN) to generate realistic images of faces.
data set

The CelebA dataset, which contains more than 200,000 images of different celebrities' faces, was used. The data set can be downloaded from this link.
Requirements

To run this project, the following packages are needed:

        lower
        zip file
        numb
        tensorflow
        matplotlib
        learn

how to run

To run this project, first clone this repository and download the CelebA dataset using the link provided. Then open a terminal and navigate to the cloned repository. Run the following command to train the GAN model:

python gan.py

Generative Adversarial Networks (GAN) Project

This project aims to create a Generative Adversarial Network (GAN) to generate realistic images of faces.
data set

The CelebA dataset, which contains more than 200,000 images of different celebrities' faces, was used. The data set can be downloaded from this link.
Requirements

To run this project, the following packages are needed:

        lower
        zip file
        numb
        tensorflow
        matplotlib
        learn

how to run

To run this project, first clone this repository and download the CelebA dataset using the link provided. Then open a terminal and navigate to the cloned repository. Run the following command to train the GAN model:

python gan.py

This will start the training process and save the generator and discriminator models to the current directory once the training is complete.
Code Explanation

The code consists of three main parts:
Part 1: Data preparation

The CelebA dataset is downloaded and unzipped using the gdown and zipfile packages. The ImageDataGenerator class in tensorflow.keras.preprocessing.image is used to load and preprocess the images.
Part 2: Modeling

The generator and discriminator models are created using tensorflow.keras.models.Sequential. The generator takes a random vector of length latent_dim as input and generates an image. The discriminator takes an image as input and generates a binary classification (true or false). Both models use Conv2DTranspose, BatchNormalization, and LeakyReLU layers.

A custom GAN class is created to combine the generator and discriminator models into a single model. The compile and train_step methods are implemented to compile and train the model.
Part 3: Model Training

The train_step method of the GAN class is used to train the GAN model. The generator is trained to generate realistic images that can fool the discriminator into classifying them as real. The discriminator is trained to correctly classify real images as real and fake images as fake.
Results

The trained GAN model is capable of generating high-quality facial images that appear almost lifelike. The quality of the generated images can be improved by training the model for a longer time or by using a larger data set.
