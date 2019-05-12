# Neural Network

__Neural networks__ are a set of algorithms, modeled loosely after the human brain, that are designed to recognize patterns. They interpret sensory data through a kind of machine perception, labeling or clustering raw input. The patterns they recognize are numerical, contained in vectors, into which all real-world data, be it images, sound, text or time series, must be translated.

The layers are made of __nodes__. A node is just a place where computation happens, loosely patterned on a neuron in the human brain, which fires when it encounters sufficient stimuli. 

![alt text]()
![image.png](data:image/jpeg;base64,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)
A node layer is a row of those neuron-like switches that turn on or off as the input is fed through the net. Each layer’s output is simultaneously the subsequent layer’s input, starting from an initial input layer receiving your data.

![alt text](https://skymind.ai/images/wiki/mlp.png)

Simply put, a neural network is a connected graph with input neurons, output neurons, and weighted edges. Let’s go into detail about some of these components:

__1) Neurons:__ A neural network is a graph of neurons. A neuron has inputs and outputs. Similarly, a neural network has inputs and outputs. The inputs and outputs of a neural network are represented by input neurons and output neurons.

__2) Connections and Weights:__ A neural network consists of connections, each connection transferring the output of a neuron to the input of another neuron. Each connection is assigned a weight.

__3) Propagation Function:__ The propagation function computes the input of a neuron from the outputs of predecessor neurons. The propagation function is leveraged during the forward propagation stage of training.

__4) Learning Rule:__ The learning rule is a function that modifies the weights of the connections. This serves to produce a favored output for a given input for the neural network. The learning rule is leveraged during the backward propagation stage of training.