# Project-Report-on-CLIP

CLIP.png has the model pipeline saved 

Install PyTorch 1.7.1+ and torchvision.Then install this repo as a Python package. On a CUDA GPU machine. 

If running on a machine without a GPU remember replace cudatoolkit=11.0 with appropriate CUDA version.

For the API: You can find CLIP module which has all the models stored inside it. And you can also load them. 

The .ipynb file in notebook folders is my implemenation trying to replicate the results. Wherein you will see 95.1% accuracy on CIFAR. 

For the improvement test run the pre-trained model by manipulating input size and parameter C on your system. 

DEMO.png has the demo image with code which specifies the tokens sent to the model for prediction. It shows the zero shot capability of the model. It doesn't require the label itself and even then it matches the best text prompt/label which shows how strong the CLIP model is. 
