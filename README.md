# GAN---Aircraft
Generative Adverserial Network model used to generate various aircraft models

This model is a simple GAN model which uses a built-from-scratch classifier and generator. Dataset is not provided in this repository could not be included to due technical issues.

The method of implementation is essentially the basic premise of a GAN model. The generator would generate several fake image of aircrafts and group in a batch with several images from the real dataset with labels stating which are false and true images. The batch is then fed to the classifier to identify. If the classifier can identify the fake images, the generator's weights would be adjusted to create better fake images. If the classifier fails however, it is the classifier's weights that are adjusted to better identify these images. Both these adjustments are determined by how much of the classifier identied right or wrong for the generator and classifier respectively.

For simplicity's sake and due to the lack of the computing power, the output of the generator is only that of a 16*16 image.
