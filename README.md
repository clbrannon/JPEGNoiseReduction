# JPEGNoiseReduction

##JPEG Artifact Reduction Model

This project is meant to create and train a Deep Learning model in order to learn to recognize how JPEG degradation affects images, and reverse the process. This necessitates the model being generative in nature. For this purpose, I've selected a UNet architecture.

###The process of training will be based on the Stable Diffusion method, with some important alterations:
    
* Instead of gaussian noise, this model will be trained on the noise specific to JPEG degadation.
* There will be no need for prompting as an input, so there will be no need for tokenization or autoencoder.
* Although it will be generative, there should be no need for a scheduler to add noise.
