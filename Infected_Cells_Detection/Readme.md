# Convolutional Neural Network (CNN) :

In neural networks, __Convolutional neural network (ConvNets or CNNs)__ is one of the main categories to do images recognition, images classifications. Objects detections, recognition faces etc., are some of the areas where CNNs are widely used.

CNN image classifications takes an input image, process it and classify it under certain categories (Eg. Infected and Uninfected cells). Computers sees an input image as array of pixels and it depends on the image resolution. Based on the image resolution, it will see __h x w x d( h = Height, w = Width, d = Dimension )__. Eg., An image of 6 x 6 x 3 array of matrix of RGB (3 refers to RGB values) and an image of 4 x 4 x 1 array of matrix of grayscale image.

![alt text](https://cdn-images-1.medium.com/max/1200/1*CBY94wikMUCZMB4-Xxs-pw.png)

The below figure is a complete flow of CNN to process an input image and classifies the objects based on values:

![alt text](https://cdn-images-1.medium.com/max/800/1*XbuW8WuRrAY5pC4t-9DZAQ.jpeg)

Convolution is the first layer to extract features from an input image. Convolution preserves the relationship between pixels by learning image features using small squares of input data. It is a mathematical operation that takes two inputs such as image matrix and a filter or kernal.
![alt text](https://cdn-images-1.medium.com/max/800/1*kYSsNpy0b3fIonQya66VSQ.png)

Consider a 5 x 5 whose image pixel values are 0, 1 and filter matrix 3 x 3 as shown in below:

![alt text](https://cdn-images-1.medium.com/max/800/1*4yv0yIH0nVhSOv3AkLUIiw.png)
Then the convolution of 5 x 5 image matrix multiplies with 3 x 3 filter matrix which is called __“Feature Map”__ as output shown in below:

![alt text](https://cdn-images-1.medium.com/max/800/1*MrGSULUtkXc0Ou07QouV8A.gif)

Convolution of an image with different filters can perform operations such as edge detection, blur and sharpen by applying filters.

__Fully Connected Layer__

The layer we call as FC layer, we flattened our matrix into vector and feed it into a fully connected layer like neural network.

![alt text](https://cdn-images-1.medium.com/max/800/1*Mw6LKUG8AWQhG73H1caT8w.png)

![alt text](https://cdn-images-1.medium.com/max/800/1*4GLv7_4BbKXnpc6BRb0Aew.png)


__About Data__

* __Overview of Data__

![image.jpg](image/Capture.PNG)<br><br>

![image.jpg](image/Capture1.PNG)<br><br>

* __Comparision of Healthy and Infected Cells__

![image.jpg](image/Capture2.PNG)<br><br>

* __Dark Spot Identification__

![image.jpg](image/Capture3.PNG)<br><br>

* __One Hot Encoding__

![image.jpg](image/Capture4.PNG)<br><br>

* __Splitting Dataset into Test-Train sample__


![image.jpg](image/Capture5.PNG)<br><br>

___

__Model 1__

* __Model Summary__

![image.jpg](image/Capture6.PNG)<br><br>

* __Confusion Matrix__

![image.jpg](image/Capture7.PNG)<br><br>

* __Classification Report__

![image.jpg](image/Capture8.PNG)<br><br>

* __Epochs v/s Loss__

![image.jpg](image/Capture9.PNG)<br><br>

* __Epochs v/s Accuracy__

![image.jpg](image/Capture10.PNG)<br><br>

__Model 2__

* __Model Summary__

![image.jpg](image/Capture11.PNG)<br><br>

* __Confusion Matrix__

![image.jpg](image/Capture12.PNG)<br><br>

* __Classification Report__

![image.jpg](image/Capture13.PNG)<br><br>

* __Epochs v/s Loss__

![image.jpg](image/Capture14.PNG)<br><br>

* __Epochs v/s Accuracy__

![image.jpg](image/Capture15.PNG)<br><br>
