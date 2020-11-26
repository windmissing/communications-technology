## Volterra级数模型

$$
\begin{aligned}
y(n) = \sum_{k=1}^K y_k(n)   \\
y_k(n) \sum_{q_1=0}^Q \cdots \sum_{q_k=0}^Q h_k(q_1, q_2, \cdots, q_k)\prod_{l=1}^K x(n-q_l)
\end{aligned}
$h_k(q_1, q_2, \cdots, q_k)$：k阶内核  
$x(n-q_l)$：输入信号  
$y(n)$：输出信号  

公式说明：  
K： 非线性的阶数  
Q： 记忆深度  
$$

优点：描述准确  
缺点：计算复杂  

## 记忆多项式模型 MP

k阶内核矩阵内保留对角线位置  
$$
y(n) = \sum_{k=1}^K\sum_{q=0}^Q h_{k,q}x^k(n-q)
$$

复基带形式：  
$$
y(n) = \sum_{k=1}^K\sum_{q=0}^Q h_{k,q} x(n-q)|x(n-q)|^{k-1}
$$

优点：  
描述准确，但计算不复杂  
只考虑奇次阶非线性，k=2l+1  

## GMP

## MPM Momery Polynomial Model

简写：  
$$
y(n) = \sum_{q=0}^Q f_q(x(n-q))
$$

$f_q$为非线性函数  
