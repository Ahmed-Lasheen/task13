# Task 13 - NN Magic


## **About**

Neural Networks are a class of machine learning algorithms inspired by the way
the human brain works, capable of processing complex data and learning from
experience. They are particularly effective in fields like image recognition,
speech processing, and even autonomous systems. In this task, you'll explore
the basics of neural networks by building one from scratch, diving into key
concepts, and applying them to a real-world problem: classifying handwritten
digits from the MNIST dataset.

## **neural networks Chapter and videos summary**
Through learning from :
- foundational concepts introduced in Michael Nielsen’s Neural Networks and Deep Learning book (Chapter 1)
- concepts introduced in the youtube video : `But what is a neural network? | Chapter 1, Deep learning` , Channel name : `3Blue1Brown`
im going to explain briefly what are the neural networks and how do they work
### 1. what are neurons :
- similar to brain's neurosystem a neuron is like a point in a web-like network 
### 2. how does it work :
- it's like a node that has specific connections with corresponding neurons only and has almost only 1 function which is output through numerical value which lies between `[ 0.0 , 1.0 ]`
### 3. how does this function work :
- it's a set of functions distributed on an array of neurons that split the given information between them then each of these neurons passes the output after it has calculated the data with already existing methods
### 4. what happens after calculation? :
- the array of neurons after finishing the split-calculations of the same information it's then passed to the next set but only after giving weights to each neuron output 
- then they are calculated by sigmoid function which sums up all the weights of the neuron array then resize the output according to the `[ 0.0 , 1.0 ]` range then it's ready to be passed to the next array of neurons
- this process continues until the last set of neurons which gives you the desired output


## **nn-from-scratch-class vs pytorch-nn-class**
### 1. ease and felixble
- `from scratch` : it's more detailed and more felixble to be edited as it's made from 0 and built up parameter by parameter , function by function , all ways of propagation are handmade : is more prone to error but it has more felixibilty
- `pytorch` : all the forward and backward propagation, gradient computation, and weight updates were handled automatically by the PyTorch framework : easy to implement and integration
### 2. Performance
- `from scratch`: The performance of the NumPy-based model is slower because it runs on the CPU without optimization for large-scale operations, which can be a bottleneck when working with larger datasets or more complex networks.
- `pytorch`: PyTorch can leverage GPU acceleration, which significantly improves performance, particularly for large-scale datasets like MNIST or when building deeper networks. The built-in optimizations in PyTorch also contribute to faster training times.
