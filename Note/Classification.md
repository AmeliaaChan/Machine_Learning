## Classification 分类算法
+ **贝叶斯公式**
\$$ P(C_1|x)=\frac{P(x|C_1)P(C_1)}{P(x|C_1)P(C_1)+P(x|C_2)P(C_2)} $$  
+ **Gaussian Distribution**
$$ f_{\mu,\Sigma}(x)=\frac{1}{(2\pi)^{D\backslash2}}\frac{1}{(|\Sigma|)^{1\backslash2}}exp\{-\frac{1}{2}(x-\mu)^T\Sigma^{-1}(x-\mu)\} $$
Input：vector x  
output：probability of sampling x  
mean $\mu$ ,covariance matrix $\Sigma$  
+ **Maximum Likelihood 最大似然**
$$ L(\mu,\Sigma)=f_{\mu,\Sigma}(x^1)f_{\mu,\Sigma}(x^2)f_{\mu,\Sigma}(x^3)...$$
$$ \mu^*,\Sigma^*=arg\ \underset{\mu,\Sigma}{max}\ L(\mu,\Sigma) $$
$$ \mu^*=\frac{1}{n}\sum_{i=1}^nx^i,\Sigma^*=\frac{1}{n}\sum_{i=1}^n(x^i-\mu^*)(x^i-\mu^*)^T$$
