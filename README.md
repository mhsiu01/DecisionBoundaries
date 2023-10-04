# DecisionBoundaries
Recreating results from Andrej Karpathy's ConvNetJS 2D toy data example (https://cs.stanford.edu/people/karpathy/convnetjs/demo/classify2d.html).
This notebook trains a simple neural net with one hidden layer made of 3 hidden units. Then I printed out the learned parameter values and rewrote the neural net as one giant function:
![CodeCogsEqn](https://github.com/mhsiu01/DecisionBoundaries/assets/78574718/d52f6c7c-e191-4b75-baea-1cdfe47610af)

We can see that the net learns a triangle-like shape, but the three corners are cut off by the interaction between the 3 hidden units:
<img width="889" alt="prob_green" src="https://github.com/mhsiu01/DecisionBoundaries/assets/78574718/a8dad300-ba2e-49a6-ba43-35a058d57000">


