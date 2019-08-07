# AlexNetArchitecture

It contains 5 convolutional layers and 3 fully connected layers. 
Relu is applied after very convolutional and fully connected layer. 
Dropout is applied before the first and the second fully connected year. 
The image size in the following architecutre chart should be 227 * 227 instead of 224 * 224, 
as it is pointed out by Andrei Karpathy in his 
famous CS231n Course. More insterestingly, the input size is 224 * 224 with 2 padding in the pytorch torch vision. 
The output width and height should be (224–11+4)/4 + 1=55.25! The explanation here is pytorch Conv2d apply floor operator to the above result, 
and therefore the last one padding is ignored.
![alt text](https://cdn-images-1.medium.com/max/1024/1*jqKHgwZ8alM3K_JRYO_l4w.png)