# Neural network for multi class classification

a.<br/>
1)	Run the code of 2 layer neural network from for multi class classification <br/>
2)	https://stackabuse.com/creating-a-neural-network-from-scratch-in-python-multi-class-classification/<br/>
3)	Go through the code and understand each line. <br/>
4)	Build the artificial dataset as shon in the blog.<br/>
5)	Take 70% data for training. 30% data for testing<br/>
6)	Build a two-layer neural network from from scratch where zo is the output.<br/>
    a)	You will have two layers. <br/>
        i)	One is hidden layers ( use 4 neurons)<br/>
        ii)	three output layer (use one output neuron)<br/>
    b)	Use sigmoid function as activation function in hidden layers<br/>
    c)	Use softmax for output layer<br/>
    d)	Use negative log likelihood loss<br/>
    e)	Derive the derivative for softmax<br/>
    f)	Calculate the derivatives for back propagation.<br/>
7)	Write codes training module for 2000 epochs to train the neural network.<br/>
8)	Now  classify  the test data using the trained neural network. <br/>
    a)	During the test, you will do only forward pass.<br/>
    b)	Argmax the forward pass output<br/>
    c)	Report your accuracy.<br/>
9)	Draw data points for training data and also plot the class boundary in 3D plot<br/>
10)	Draw data points for test data and also plot the class boundary in 3D plot<br/>
11)	You cannot use any built-in deep learning functions<br/>
<br/>
<br/>
b. (same as a. But the input is 3X32X32 image, output 10 classes.. And three layer neural network<br/>
<br/>
1)	Download and read train data from CIFAR 10 from 10 classes<br/>
2)	Now, read one image, reshape it to row vector x. x is our input data now with dimension 1X3072.<br/>
3)	x’s class label would be one hot encoded<br/>
4)	Use two hidden layer and one output layer.<br/>
5)	Build a three-layer neural network from scratch <br/>
    a)	You will have three layers. <br/>
        i)	  First   hidden layers ( use 1000 neurons)  <br/>
        ii)	  Second hidden layers (use 100 neurons)<br/>
        iii)	Output layers (10 output neurons)<br/>
    b)	So. Output-probability:<br/>
        ao = softmax (  W<sub>o</sub> *  sigmoid  (  W<sub>h2</sub>  * sigmoid(W<sub>h1</sub>  * x + b<sub>h1</sub>)  +  b<sub>h2</sub> )  +    b<sub>o</sub> ) <br/>
    c)	Where  x is input vector,  W<sub>h1</sub>, and W<sub>h2</sub> are weight matrices for hidden layers. W<sub>o</sub> is the weight matrix for output layers. b<sub>h1</sub>,  b<sub>h2</sub>, and b<sub>o</sub> are bias vectors for corresponding layers.<br/>
    d)	Use sum of cross entropy  as your loss function. ao is the output vector.<br/>
    e)	Derive and Calculate the derivatives for back propagation for the three layer neural network.<br/>
6)	Write codes for training module for 10 epochs to train the neural network.<br/>
7)	Report your accuracy on the test set<br/>
8)	Show confusion matrix of your test prediction<br/>
9)	You cannot use any built-in deep learning functions<br/>
<br/>
<br/>
c. (use functions) – <br/>
<br/>
1)	Download and read train data from CIFAR 10 from 10 classes<br/>
2)	Same as assignment b.<br/>
3)	Write forward(X) function to implement the forward calculation.<br/>
4)	Use forward function to pass the input data to calculate the probabilities.<br/>
5)	Calculate the loss using criterion function with cross entropy option.<br/>
6)	Using the loss,  use autograd and backward()  to calculate the derivatives automatically.<br/>
7)	Write codes for training module for 10 epochs to train the neural network.<br/>
8)	Report your accuracy on the test set<br/>
9)  Show confusion matrix of your test prediction<br/>

<br/>
