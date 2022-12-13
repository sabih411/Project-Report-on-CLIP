# Project-Report-on-CLIP

CLIP.png has the model pipeline saved 

Install PyTorch 1.7.1+ and torchvision.Then install this repo as a Python package. On a CUDA GPU machine. 

If running on a machine without a GPU remember replace cudatoolkit=11.0 with appropriate CUDA version.

For the API: You can find CLIP module which has all the models stored inside it. And you can also load them. 

The .ipynb file in notebook folders is my implemenation trying to replicate the results. Wherein you will see 95.1% accuracy on CIFAR. 

Tried experimenting with different image resolution to test if reducing the size helps model to get improved accuracy since for CIFAR10 we are interpolating the samples. The experimented showed that the model couldn't scale for lower resolutions which might be because of the training code which was done on the fixed size of 224. Also authors showed that the results on cifar were dependent on the logistic regression parameter C, I tried manipulating that to reach 95% accuracy mark.

DEMO.png has the demo image with code which specifies the tokens sent to the model for prediction. It shows the zero shot capability of the model. It doesn't require the label itself and even then it matches the best text prompt/label which shows how strong the CLIP model is. 
