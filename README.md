# MNIST-Digit-Generator-GAN (MNIST Dataset)

## Description

A Generative Adversarial Network (GAN) built using TensorFlow to generate realistic handwritten digits based on the MNIST dataset. 
The generator creates digit-like images, while the discriminator learns to distinguish between real and fake images, improving the quality of generated digits over time.

## Project Structure

- **Generator**: A neural network that generates fake digit images from random noise.
- **Discriminator**: A neural network that attempts to distinguish between real and fake digit images.
- **Training**: The generator and discriminator are trained together in an adversarial setup, where the generator tries to fool the discriminator, and the discriminator tries to correctly classify real and fake images.

## Requirements

- **Python 3.x**
- **TensorFlow 2.x**
- **NumPy**
- **Matplotlib**

## Usage

To train the GAN and generate handwritten digits, run the training script:

```
train_gan(generator, discriminator, gan, train_dataset, epochs=1000)
```
Note: The number of epochs has been reduced to 1000 for quicker training.
Increasing the number of epochs will significantly improve the accuracy of the model and result in better image generation.

## How It Works
- **Data Loading**: The MNIST dataset is normalized and used for training the GAN.
- **Generator**: Produces images from random noise.
- **Discriminator**: Learns to identify real and generated images.
- **Training Loop**: The generator and discriminator are trained iteratively to improve their performance.
- **Output**: The generated images become clearer and more digit-like as training progresses.

## Output Example
Initially, the generator produces random noise images, but as training continues, it learns to generate realistic handwritten digits similar to the MNIST dataset.

## Future Improvements
- **Increase Epochs**: To enhance the image quality, increase the number of epochs during training.
- **Hyperparameter Tuning**: Adjust learning rates and other hyperparameters for more stable training.
