# Comparison of different optimizers for CNN

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/voiculaura/)](https://www.linkedin.com/in/voiculaura/)

In this notebook I'd like to compare the performance of different optimizers on a given problem. I will use the fake news dataset and the features extracted in that project using TF-IDF. The architecture of convolutional neural network is the one that gave the best performance for the fake news dataset. I have been using neural networks for a while now. However, one thing that I've always wonderd about is the selection of an optimizer for training the network (using backprop).

**SGD**

Stochastic gradient descent is very basic and is seldom used now. One problem is with the global learning rate associated with the same. Hence it doesn't work well when the parameters are in different scales since a low learning rate will make the learning slow while a large learning rate might lead to oscillations. Also Stochastic gradient descent generally has a hard time escaping the saddle points. Adagrad, Adadelta, RMSprop, and Adam generally handle saddle points better. SGD with momentum renders some speed to the optimization and also helps escape local minima better.

**AdaGrad**

Momentum adds updates to the slope of our error function and speeds up SGD in turn. AdaGrad adapts updates to each individual parameter to perform larger or smaller updates depending on their importance.

**RMSProp**

For non-convex problems, AdaGrad can prematurely decrease the learning rate. We can use an exponentially weighted average for gradient accumulation.

**AdaDelta**

AdaDelta, RMSProp almost works on similar lines with the only difference in Adadelta you don't require an initial learning rate constant to start with.

**Adam**

Adam is a combination of RMSprop and momentum (similarly, Nadam refers to a combination of RMSprop and Nesterov momentum). Adam refers to adaptive moment estimation, and it is the most popular optimizer used for neural networks today. Adam computes adaptive learning rates for each parameter. In addition to storing an exponentially decaying average of past squared gradients like Adadelta and RMSprop, Adam also keeps an exponentially decaying average of past gradients, similar to momentum.

## Contributing

I use this for my own projects, I know this might not be the perfect approach for all the projects out there. If you have any ideas, just [open an issue][issues] and tell me what you think.

If you'd like to contribute, please fork the repository and make changes as you'd like. Pull requests are warmly welcome.

## License

Distributed under the MIT License. See `LICENSE` for more information.
