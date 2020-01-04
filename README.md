# B-W-to-Color
A program which can colour black and white (grey) images. 

Converting images from grey scale to RGB is not a simple procedure because a single grayscale image may correspond to many plausible colored images. Here, we are using a auto-encoder (deep neural network) to achieve this task. 

### Problem Statement
We have gray images (single channel) that needs to be converted to colored ones. The model that we have built accepts grey images as inputs. We'll make use of the LAB color space here in our project. In this color space, the 'L' channel is nothing but the lightness (grey) channel. The other two channel (A and B) takes care of the color representataion. We train our model so that it outputs these two channels. We then use these images in the 'LAB' colorspace to get back our images in the RGB colorspace. 

The training data that I have used today is from MIT. Link is given below. 
http://places2.csail.mit.edu/download.html

#### Results
Observing the sample results, we can say that our network is doing pretty good on colouring trees, clouds, etc. One possible reason is because there are many such images in the dataset and hence the network was able to learn them well.  
