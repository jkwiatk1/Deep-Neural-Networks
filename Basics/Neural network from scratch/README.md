Neural networks from scratch.

# Used data
The collection under study is MNIST, a collection of 28x28 monochrome images showing written numerals along with labels as to what the numerals are. 
There are 70,000 images, and they have been divided into test and train datasets.

# Experiments
Experiments were conducted for the following settings:
* different values of learning rate 0.1 ; 0.2 ; 0.3 ; 0.4,
* different numbers of layers: [784,128,10], [784,256,64,10]
* training and test collection divided 85% to 15%,
* 1000 epochs,
* accuracy and mse measurement after each epoch.