# DecisionBoundaries
Recreating results from Andrej Karpathy's ConvNetJS 2D toy data example (https://cs.stanford.edu/people/karpathy/convnetjs/demo/classify2d.html).
This notebook trains a simple neural net with one hidden layer made of 3 hidden units. Then I printed out the learned parameter values and rewrote the neural net as one giant function:
<img src="https://latex.codecogs.com/svg.image?\huge&space;\bg{white}\frac{e^{-1.6584\cdot\max\left(0,2.2073x-0.4897y-0.9715\right)-1.3337\cdot\max\left(0,-1.4752x-1.6321y-0.9149\right)-1.3917\cdot\max\left(0,-0.6496x&plus;2.0777y-0.801\right)&plus;2.4065}}{e^{-1.6584\cdot\max\left(0,2.2073x-0.4897y-0.9715\right)-1.3337\cdot\max\left(0,-1.4752x-1.6321y-0.9149\right)-1.3917\cdot\max\left(0,-0.6496x&plus;2.0777y-0.801\right)&plus;2.4065}&plus;e^{1.7072\cdot\max\left(0,2.2073x-0.4897y-0.9715\right)&plus;1.9719\cdot\max\left(0,-1.4752x-1.6321y-0.9149\right)&plus;1.8006\cdot\max\left(0,-0.6496x&plus;2.0777y-0.801\right)-2.5301}}" title="\frac{e^{-1.6584\cdot\max\left(0,2.2073x-0.4897y-0.9715\right)-1.3337\cdot\max\left(0,-1.4752x-1.6321y-0.9149\right)-1.3917\cdot\max\left(0,-0.6496x+2.0777y-0.801\right)+2.4065}}{e^{-1.6584\cdot\max\left(0,2.2073x-0.4897y-0.9715\right)-1.3337\cdot\max\left(0,-1.4752x-1.6321y-0.9149\right)-1.3917\cdot\max\left(0,-0.6496x+2.0777y-0.801\right)+2.4065}+e^{1.7072\cdot\max\left(0,2.2073x-0.4897y-0.9715\right)+1.9719\cdot\max\left(0,-1.4752x-1.6321y-0.9149\right)+1.8006\cdot\max\left(0,-0.6496x+2.0777y-0.801\right)-2.5301}}" />

We can see that the net learns a triangle-like shape, but the three corners are cut off by the interaction between the 3 hidden units:
<img width="889" alt="prob_green" src="https://github.com/mhsiu01/DecisionBoundaries/assets/78574718/a8dad300-ba2e-49a6-ba43-35a058d57000">


