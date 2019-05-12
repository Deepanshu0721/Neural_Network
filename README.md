# Neural Network

__Neural networks__ are a set of algorithms, modeled loosely after the human brain, that are designed to recognize patterns. They interpret sensory data through a kind of machine perception, labeling or clustering raw input. The patterns they recognize are numerical, contained in vectors, into which all real-world data, be it images, sound, text or time series, must be translated.

The layers are made of __nodes__. A node is just a place where computation happens, loosely patterned on a neuron in the human brain, which fires when it encounters sufficient stimuli. 

![alt text](data:image/png;base64,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)

A node layer is a row of those neuron-like switches that turn on or off as the input is fed through the net. Each layer’s output is simultaneously the subsequent layer’s input, starting from an initial input layer receiving your data.

![alt text](https://skymind.ai/images/wiki/mlp.png)

Simply put, a neural network is a connected graph with input neurons, output neurons, and weighted edges. Let’s go into detail about some of these components:

__1) Neurons:__ A neural network is a graph of neurons. A neuron has inputs and outputs. Similarly, a neural network has inputs and outputs. The inputs and outputs of a neural network are represented by input neurons and output neurons.

__2) Connections and Weights:__ A neural network consists of connections, each connection transferring the output of a neuron to the input of another neuron. Each connection is assigned a weight.

__3) Propagation Function:__ The propagation function computes the input of a neuron from the outputs of predecessor neurons. The propagation function is leveraged during the forward propagation stage of training.

__4) Learning Rule:__ The learning rule is a function that modifies the weights of the connections. This serves to produce a favored output for a given input for the neural network. The learning rule is leveraged during the backward propagation stage of training.
