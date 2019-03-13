## Stochastic Gradient Descent in Python  

Gradient Descent is an optimization algorith that is widely used in machine learning and deep learning to optimize& reduce our loss by adjusting the weights of our model/algorithm. Partial derivatives are the heart of this optimization algorithm. Without partial derivatives, optimization fails!!

## What we do in GradientDescent?

Our job is to minimize the loss of our model and the only tunable parameters excluding the hyperparameters are the weights and biases of our model, Our inputs are constant as we know. We first calculate how sensitive our loss function is w.r.t our weights i.e In what way changing our weights change our loss function (This is finding partial derivatives of our weights with respect to our losses). If the changing the weights in a small way in a particular direction accounts for reduction in loss function, We will go and make the changes to the weights through Gradient Descent update step(most important equation in GradientDescent). If the change in the direction accounts for increase in loss of our model, We donot update it.

Till we were working with one weight. Consider if there are 1000's of weights. We for sure know that there is certain way as per which if we change all those 1000's of weights we can observe an overall reduction in loss of our model OR These is sweet value for each of our weights that if we somehow are able to find the sweet value, We will be able to reduce our loss. That is precisely what will we doing in Gradient Descent
