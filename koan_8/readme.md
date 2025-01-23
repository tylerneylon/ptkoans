# Koan 8 — Train a variational autoencoder (VAE)

## The Question
How can you build and train a variational autoencoder in pytorch?

## Sample Data
I suggest starting the Fashion MNIST dataset. This data contains 28x28
grayscale images of articles of clothing. Here are some example images:

![sample images from Fashion MNIST](fashion-mnist-sprite.png)

This is labeled data, with ten labels like "coat", "sneaker" or "ankle boot."
However, autoencoders (including VAEs) don't use labels, so you won't use those
during training — though you could use them to evaluate the resulting model.

There are 60k training images and 10k test images. This dataset can be
[downloaded separately](https://github.com/zalandoresearch/fashion-mnist),
though you might as well use the interface that's
conveniently built in to `torchvision`:

```
from torchvision import datasets, transforms

transform = transforms.Compose([transforms.ToTensor()])

train_dataset = datasets.FashionMNIST(
        root='./data', train=True,  transform=transform, download=True)
test_dataset  = datasets.FashionMNIST(
        root='./data', train=False, transform=transform, download=True)
```

## Architecture

TBD

## Tricky Points

TBD






