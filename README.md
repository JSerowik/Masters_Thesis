Masters_Thesis
Dual Capsule Neural Network (CapsNet) Generative Adversarial Network (GAN) 
(DCN-GAN)

My ongoing Masters' thesis is studying the viability of using a Capsule Neural Network as a Generator in a GAN model. Generating from the output of a CapsNet was proposed in the original paper 'Dynamic Routing Between Capsules' (https://arxiv.org/abs/1710.09829). In order to accomplish this a CapsNet was trained for classification and the output of a single class in the DigitCaps layer was input into a simple Dense Decoder and trained to generate an image from this output. What I wish to accomplish is diffenrent in that I want to create a CapsNet generator without having to train the network to classify images, in other words have a "Semi-supervised" CapsNet Generator. Initial tests have confirmed the viability of this while also using a CapsNet as a Critic/Discriminator on the MNIST data set. I have noticed some volitility while training and am looking to implement ways of improving this (Wasserstein loss possibly). I also have experimented with a slightly modified CapsNet Generator architecture for the CIFAR-10 data set and have found success. The Jupyter Notebook here is just a helpful guide for anyone interested in the topic and I would greatly appreciate feedback.


Credit to:
- Xifeng Guo for the excellent implementation which I heavily modified for the generator network (https://github.com/XifengGuo/CapsNet-Keras)
- Raeid Saqur for the well documented CapsNet discriminator in his paper and Github library (https://github.com/raeidsaqur/CapsGAN)