<html>
<body>
<h3> MNIST dataset classification with out libraries </h3>
<p> MNIST is a large database of handwritten digits. In this project MNIST dataset is trained using Neural Networks and to achieve this any special libraries like Theano or scikit learn etc. are not used rather 'scipy.optimize.fmin_cg' function is used to minimize the cost function of algorithm. 
This scipy.optimize.fmin_cg function takes 2 inputs mainly: </br> 1.  A Function which returns cost function of neural nets at given weights and </br>
2. A function which returns gradient of weights. Backpropogation algorithm is used to calculate gradient of weights. </br> In special libraries like Theano or scikit learn etc. we do not have to explicity give function to calculate gradient of weights. </br> Neural network contains 4 layers: </br>
1. Input layer contains 28X28 neurons </br>
2. Hidden layer-1 contains 300 units </br>
3. Hidden layer-2 contains 300 units </br>
4. Output layer contains 10 neurons (as 10 classes). </br> Quadratic cost function , sigmoid activation function and Gradient descent is used to minimize cost function in this project. </br>
</p>
<h3> About files in this project </h3>
<p>
<b>ExtractingData.py:</b> To extract training images and labels from 'train-images-idx3-ubyte' and 'train-labels-idx1-ubyte' packages respectively</br>
<b>ExtractingTestData.py:</b> To extract testing images and labels from 't10-images-idx3-ubyte' and 't10-labels-idx1-ubyte' packages respectively</br>
<b>CostFunction.py</b> Returns the cost of neural network for given weights</br>
<b>WeightsGradient.py</b> Returns gradient of weights for given weights</br>
<b>sigmoid.py</b> Returns sigmoid activation function </br>
<b>sigmoidGradient.py</b> Returns gradient if sigmoid activation function </br>
<b>RandomInitializeWeights.py</b> Radomly initializes weights of given size</br>
<b>ComputeNumericalGradient.py</b> Returns numerical gradient of weights which is given by dy/dx = (y2-y1)/(x2-x1)</br>
<b>DebugInitialWeights.py</b> Returns randomly initialized weights of given size but weights generated using this program as opposed to weights generated by RandomInitializeWeights.py are used to check if the gradient value returned by WeightsGradient.py is close to gradient value retuned by ComputeNumericalGradient.py </br>
<b>CompareNeuralNetGradientWithNumericalGradient.py</b> This programs is used to check if the gradient value returned by WeightsGradient.py is close to gradient value retuned by ComputeNumericalGradient.py </br>
<b>MNISTTraining.py</b>This program learns weights in such a way that the cost function of neural networks is minimized and thus increase accuracy with each iteration. 'scipy.optimize.fmin_cg' is used to minimize the cost function </br>
</p>
<h3> Sample code to run program </h3>
<p> import MNISTTraining </p>
<h3> Accuracy </h3>
Accuracy of 93.2% was attained after running the algorithm for 150 iterations. Weights with which this accuracy was achievied are stored in weights.npy
<p> </p>
</body>
</html>

 

