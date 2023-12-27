## Regression - Case Study
### Step1.Model  
  a set of function  
### Step2.Goodness of Function    
+ **Loss function L**  
Input：a function，output：how bad it is  
### Step3.Best Function
+ **Gradient Descent 梯度下降**  
  + 一个参数w：
    <div align=center><img src="https://github.com/AmeliaaChan/Machine_Learning/blob/main/Note/Image/Reg1.png" height="400px"></div>
  + 两个参数w&b:
    <div align=center><img src="https://github.com/AmeliaaChan/Machine_Learning/blob/main/Note/Image/Reg2.png" height="400px"></div>  
    Don't worry. In linear regression,the loss function is convex/no local optimal  
+ **Selecting suitable Model**  
**Overfitting 过拟合**：A more complex model dose not always lead to better performance on testing data.  
### Back to step1.Redesign Model  
### Back to step2.Regularization 正则化  
+ Redesign loss function
  <div align=center><img src="https://github.com/AmeliaaChan/Machine_Learning/blob/main/Note/Image/Reg3.png" height="200px"></div>
  不考虑bias，bias与平滑度无关  
  We prefer smooth function,but don't be too smooth.  
### Conclusion  
+ Gradient descent  
+ Overfitting and Regularization  
