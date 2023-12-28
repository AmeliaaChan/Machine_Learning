## Classification 分类算法
+ **贝叶斯公式**
$$ P(C_1|x)=\frac{P(x|C_1)P(C_1)}{P(x|C_1)P(C_1)+P(x|C_2)P(C_2)} $$  
+ **Gaussian Distribution**
$$ f_{\mu,\Sigma}(x)=\frac{1}{(2\pi)^{D\backslash2}}\frac{1}{(|\Sigma|)^{1\backslash2}}exp\{ -\frac{1}{2}(x-\mu)^T\Sigma^{-1}(x-\mu)\} $$
Input：vector x  
output：probability of sampling x  
mean $\mu$ ,covariance matrix $\Sigma$  
+ **Maximum Likelihood 最大似然**  
$$ L(\mu,\Sigma)=f_{\mu,\Sigma}(x^1)f_{\mu,\Sigma}(x^2)f_{\mu,\Sigma}(x^3)...$$    
$$ \mu^{* },\Sigma^{* }=arg\underset{\mu,\Sigma}{max}L(\mu,\Sigma)$$  
$$ \mu^{* }=\frac{1}{n}\sum_{i=1}^nx^i,\Sigma^{* }=\frac{1}{n}\sum_{i=1}^n(x^i-\mu^{* })(x^i-\mu^{* })^T $$
+ **Modifying Model**  
Find $\mu^1,\mu^2,\Sigma$ maximizing the likelihood $L(\mu^1,\mu^2,\Sigma)$
$$ L(\mu^1,\mu^2,\Sigma)=f_{\mu^1,\Sigma}(x^1)f_{\mu^1,\Sigma}(x^2)...f_{\mu^1,\Sigma}(x^{79})\times f_{\mu^2,\Sigma}(x^{80})f_{\mu^2,\Sigma}(x^{81})...f_{\mu^2,\Sigma}(x^{140})$$
$\mu^1$ and $\mu^2$ is the same，$\Sigma=\frac{79}{140}\Sigma^1+\frac{61}{140}\Sigma^2$  
---
### Three Steps  
+ **Fuction Set(Model)**  
运用贝叶斯公式
+ **Goodness of a function**  
最大似然
+ **Find the best funcion:easy**  
---
+ **Probability Distribution**  
For binary features,you may assume they are from Bernoulli distributions.  
If you assume all the dimensions are independent,then you are using Native Bayes Classifier.（朴素贝叶斯）  
+ **Posterior Probability**  
Sigmoid function  
<div align=center><img src="https://github.com/AmeliaaChan/Machine_Learning/blob/main/Note/Image/Cla1.png?raw=true" width="400px"><div\>  
<div align=center><img src="https://github.com/AmeliaaChan/Machine_Learning/blob/main/Note/Image/Cla2.png?raw=true" width="400px"><div\>  

Then we just need w and b.




