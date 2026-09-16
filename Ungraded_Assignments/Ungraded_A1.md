# UNgraded Assignment 1: Neural Networks for Structured Data or Tabular data
###  You can do this assignment in Google Colab (which runs on cloud), or lab computer. YOu will need a google account, the free version of Colab is sufficient to run these toy models. https://research.google.com/colaboratory/faq.html
Feed Forward Neural Network (FFNN) / Multi-layer Perceptrons (MLP)
References:
* Chapter 13, Probabilistic Machine Learning: An Introduction by Kevin Murphy  

---
# **AI and Human Policy**
* **Use of AI for 'Review' sections**
  * YOU CAN use it to understand concepts and sections of the code that are new to you
* **Use of AI for sections 'Questions' and 'Programming exercises'**
  * YOU CAN use to it verify your responses, or find more efficient ways of coding
  * DO NOT use it to directly find answers or write the full code.
* **Discussions with humans**
  * YOU CAN 'discuss' with your classmates
  * DO NOT 'copy'

* **GRADING**: 10% of overall grades is for class participation (submission of ungraded assignments).

___
# 1. REVIEW
1. Review 2_Lecture_NN_tabular data_Basics.ipynb
2. Review 2a_Code_NN_Backprop_SymbolicDiff.ipynb
    * We explicitly coded backprop (no in-built package)
    * We set NN architecture to one hidden layer - number of nodes in the hidden layer was a user input
    * We used symbolic differentiation
3. Review 2c_Code_NN_Backprop_AutoDiff.ipynb
    * Same as 2b except uses Auto diff
4. Review 2d_Code_NN_PyTorch_Basic.ipynb
    * Uses Pytorch library (in-built package)


---

# 2. EXPERIMENT

* Plots of predicted v. actual fit are used here to evaluate model fit. This may not always be feasible. Loss function is more appropriate. How to track Loss function under different hyperparameter sets?
  * Tensorboard helps track this.  (Weights and Biases is another software that is commonly used). The code has been setup to use Tensorboard
* Hyperparameter tuning: Modify hidden layer size (number of nodes in hidden layer), learning rate, epochs
* In 2a, 2c - Initialize weights to very high and very low values
* Get under the hood to understand of the math of how it works   
  * IN 2c observe plots of Hidden node outputs: To fully understand the role of activation functions, plot both 'input's to hidden node, and 'outputs' from hidden node
  * Play with
 [Tensor playground](https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.02424&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false)

---

# 3. SUBMIT: PROGRAMMING EXERCISE  - MIE 625 (recommended for 525)

* Modify 2a or 2c code to use two hidden layers. First derive the differential equations (keep Sigmoid activation), and then code it
---

# 4. SUBMIT: PROGRAMMING EXERCISE - MIE 625 and 525
  * Use 2d (or your own code) Fit a model for a slightly more complex function: $y=sin(x)$ or $y=x_1^2 +x_2^2$ ( generate synthetic data for model training).
  * Modify the code to Hyperparameter tune using RandomizedSearchCV (see Eden Vachtel's thesis code -in A1_Graded folder). It is a scikit-learn package https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html .  2d_code uses PyTorch for NN module, so !pip install to install necessary packages. You can use AI to give you an example, use that as a guide to code it into 2d_code.

# SUBMISSION GUIDELINES: Submit.ipynb files. Run the code before submitting so the outputs are visible. 
  
