### Section 6.4 Binomial Coefficients
pg443: 4, 7, 8, 9

4\. Find the coefficient of $x^5y^8$ in $(x + y)^{13}$.
>Solution
$$
\begin{aligned}
(x+y)^{13} &= \sum^{13}_{k=0}\binom{13}{k}x^{13-k}y^k\\
k=8 \To \text{the coefficient of }x^5y^8 \text{ is } \binom{13}{8} &= \frac{13!}{5!8!}
\end{aligned}
$$

7\. What is the coefficient of $x^9$ in $(2-x)^{19}$?
>Solution
$$
\begin{aligned}
(2-x)^{19} &= \sum^{19}_{k=0}\binom{19}{k}2^{19-k}(-x)^k\\
k &= 9 \To \text{the coefficient of }x^9\text{ is } \binom{19}{9} \cdot 2^9 \cdot (-1)^9= -\frac{2^9\cdot 19!}{10!9!}
\end{aligned}
$$

8\. What is the coefficient of $x^8y^9$ in the expansion of $(3x + 2y)^{17}$?
>Solution
$$
\begin{aligned}
(3x+2y)^{17} &= \sum^{17}_{k=0}\binom{17}{k}(3x)^{17-k}(2y)^k\\
k &= 9 \To \text{the coefficient of }x^8y^9 \text{ is } \binom{17}{9} \cdot 3^8 \cdot 2^9= \frac{3^8 \cdot 2^9 \cdot 17!}{8!9!}
\end{aligned}
$$

9\. What is the coefficient of $x^{101}y^{99}$ in the expansion of $(2x-3y)^{200}$?
>Solution
$$
\begin{aligned}
(2x-3y)^{200} = \sum^{200}_{k=0}\binom{200}{k}(2x)^{200-k}(-3y)^k\\
k=99 \To \text{the coefficient of }x^{101}y^{99} \text{ is } \binom{200}{99} \cdot 2^{101} \cdot (-3)^{99}= -\frac{2^{101} \cdot 3^{99} \cdot 200!}{101!99!}
\end{aligned}
$$
