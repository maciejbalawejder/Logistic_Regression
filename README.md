![MEME](https://github.com/maciejbalawejder/Logistic_Regression/blob/main/i-know-logistic-regression-show-me.jpg)
# Logistic Regression

### Model of Logistic Regression bulit from scratch in educational purpose(to avoid situtation from the meme above) which tries to be small and clean. It is not complicated model, containing only 115 lines of code, and explaining in depth operation which are going "behind the scenes" when you use libraries like sklearn. Two init arguments are taken, iterations and learning rate. The rest of the code is explained in depth below. 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Main functions : 
#### 1) Sigmoid - 1/(1+e^(-input•weights))
![Sigmoid](https://github.com/maciejbalawejder/Logistic_Regression/blob/main/sigmoid.png)
The function is squashing values and keep them between(0,1).
#### 2) Split - takes two arguments dataset and seprator
#### 3) Cost - Cross-Entropy function  C=−1n∑x[yln(a)+(1−y)ln(1−a)] | a = input•weights, for traning set and validation set
        Yeah, but why cross-entropy? 
        The bigger error between predicted output and ground truth the more it affects the loss function(more than MSE cause it is logarithmic) and forces to update weights to     
        achive opposite result
#### 4) Update - updates the weights W[i] = W[i-1] - learning_rate * dJ/dW
#### 5) Predict - gives a predicted values based on trained weights and given inputs(X) 
        OUTPUT = X • Weights
#### 6) Fit - takes two arguments X - inputs, and y - ground truth 
        For number of iterations the based on given X, y the loss function and updating weights is executed.
        
### Fixed :
* confusion matrix
* cost
* updating weights 

### To do :
* scalling data
* optimizing model
  * [x] regularization - improves generalization 
  * [x] validation dataset
  * [x] split function 
  * [x] plot learning curve
  * [x] F1 - score 
  * k-fold validation set sounds cool
 

