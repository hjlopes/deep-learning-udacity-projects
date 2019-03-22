# Project Overview

In this project a Deep Convolutional Generative Adversarial Networks (DGAN) is developed in order to generate "face" celebrity faces.

The best results results were achieved with 4 layer Discriminator and Generator with layer depths of 64.

A sample of the results after 50 epochs can be seen here:

![alt text](assets/generated_faces.png "Best results")

## Used Tricks
1. **Label smoothing:**
 Real labels are replaced with a number between 0.8 and 1.1.
 Fake labels are replaced with a number between 0 and 0.3.
2. **Dropout layers** in the the Discriminator and Generator
3. Initialize weights with Gaussian distribution

## Project instructions

Please download the learning data from [here](https://s3.amazonaws.com/video.udacity-data.com/topher/2018/November/5be7eb6f_processed-celeba-small/processed-celeba-small.zip) and extract the data into `processed_celeba_small` folder. In alternative uncomment and run the first line in the jupyter notebook:
```ipnbpython
!unzip processed_celeba_small.zip
```
Launch the jupyter notebook server with:
```ipnbpython
jupyter notebook dlnd_face_generation.ipynb
```

## References

1. https://arxiv.org/pdf/1611.07004v1.pdf
2. https://github.com/soumith/ganhacks
