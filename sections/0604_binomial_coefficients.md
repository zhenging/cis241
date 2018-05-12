### 6.4 Binomial Coefficients
p436

**THE BINOMIAL THEOREM** Let $x$ and $y$ be variables, and let n be a nonnegative integer. Then
$$
\begin{aligned}
(x+y)^n &= \binom{n}{0}x^ny^0 + \binom{n}{1}x^{n-1}y^1 + \cdots + \binom{n}{n}x^0y^n\\
&=\sum^n_{k=0}x^{n-k}y^k
\end{aligned}
$$

#### Examples
1-4

#### Homework
p443: 4, 7, 8, 9

4\. Find the coefficient of $x^5y^8$ in $(x + y)^{13}$.
>Solution
$$
(x+y)^{13} = \sum^{13}_{k=0}\binom{13}{k}x^{13-k}y^k
$$
The coefficient of $x^5y^8$ is $\tbinom{13}{8} = \frac{13!}{5!8!}$.

7\. What is the coefficient of $x^9$ in $(2-x)^{19}$?
>Solution
$$
(2-x)^{19} = \sum^{19}_{k=0}\binom{19}{k}2^{19-k}(-x)^k
$$
The coefficient of $x^9$ is $\tbinom{19}{9} \cdot 2^{10} \cdot (-1)^9= -\frac{2^9\cdot 19!}{10!9!}$.

8\. What is the coefficient of $x^8y^9$ in the expansion of $(3x + 2y)^{17}$?
>Solution
$$
(3x+2y)^{17} = \sum^{17}_{k=0}\binom{17}{k}(3x)^{17-k}(2y)^k
$$
The coefficient of $x^8y^9$ is $\tbinom{17}{9} \cdot 3^8 \cdot 2^9= \frac{3^8 \cdot 2^9 \cdot 17!}{8!9!}$.

9\. What is the coefficient of $x^{101}y^{99}$ in the expansion of $(2x-3y)^{200}$?
>Solution
$$
(2x-3y)^{200} = \sum^{200}_{k=0}\binom{200}{k}(2x)^{200-k}(-3y)^k
$$
The coefficient of $x^{101}y^{99}$ is $\tbinom{200}{99} \cdot 2^{101} \cdot (-3)^{99}= -\frac{2^{101} \cdot 3^{99} \cdot 200!}{101!99!}$.
