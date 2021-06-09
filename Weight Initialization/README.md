# Comparison of different weight initializations for CNN

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/voiculaura/

In this notebook I'd like to check the effect of weight initialization on a given problem. I will use the fake news dataset and the features extracted in that project using TF-IDF. The architecture of convolutional neural network is the one that gave the best performance for the fake news dataset.

There are a number of important, and sometimes subtle, choices that need to be made when building and training a neural network. We have to decide which loss function to use, how many layers to have, what stride and kernel size to use for each convolution layer, which optimization algorithm is best suited for the network, etc. With so many things that need to be decided, the choice of initial weights may, at first glance, seem like just another relatively minor pre-training detail, but weight initialization can actually have a profound impact on both the convergence rate and final quality of a network.

In order to illustrate this fact, I’ve trained the same neural network using three different weight initialization strategies.

## Contributing

I use this for my own projects, I know this might not be the perfect approach for all the projects out there. If you have any ideas, just [open an issue][issues] and tell me what you think.

If you'd like to contribute, please fork the repository and make changes as you'd like. Pull requests are warmly welcome.

## License

Distributed under the MIT License. See `LICENSE` for more information.
