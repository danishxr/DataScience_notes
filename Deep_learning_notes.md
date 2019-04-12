## Basics Of Neural Networks 

---

The learning is respect to a binary problem.



Suppose we have an image of dimension $64*64*3$ we have to flatten it. 

So the result is an array $x$ containing 12288 parameters. 

This is for single image $x_i$ and we label $y_i$ as $1$ or $0$  

such that for $(x,y)$  $x \in R^{n_x} , y \in {0,1}$ 

like this we have $m$ training examples: $(x^{(1) }, y^{(1)}) , (x^{(2) }, y^{(2)}),(x^{(1) }, ----- , (x^{(m) }, y^{(m)})$ 

---

##### Logistic Regression 

---

Objective is Given $x​$, we want $\hat{y} = P( y=1|x)​$

If it were linear regression we would be having $\hat{y} = w^T x +b$

But we need to restrict it into $1$ & $0$ . As linear equation can go negative and also more than $1$.

 So we use sigmoid function  to wrap this linear entity.

Sigmoid function is given by $ \sigma(z) = \frac{1}{1 + e^{-z}}​$

where $z= w^T x+ b$



If $z$ is very large  $\sigma{(z)} = \frac{1}{1+0}$ as $e$ to the large number is zero. so we get $1$.

If $z$ is very large negative number   $\sigma{(z)} = \frac{1}{1+e^{-z}}$ similar to $\sigma{(z)} = \frac{1}{1+bignumber}$ which is close to $0$.

 





