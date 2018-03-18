### Section 8.2 Solving Linear Recurrence Relations
pg545: 2, 4a,d,e,f,g, 8, 12, 14

2\. Determine which of these are linear homogeneous recurrence relations with constant coefficients. Also, find the degree of those that are.
a. $a_n=3a_{n-2}$ &emsp; b. $a_n=3$
c. $a_n=a_{n-1}^2$ &emsp; d. $a_n=a_{n-1} + 2a_{n-3}$
e. $a_n=a_{n-1}/n$
f. $a_n=a_{n-1} + a_{n-2} + n + 3$
g. $a_n=4a_{n-2} + 5a_{n-4} + 9a_{n-7}$
>Solution
a. Linear, homogeneous, constant coefficient, and degree of 2.
b. Not recurrence relations.
c. Not linear.
d. Linear, homogeneous, constant coefficient, and degree of 3.
e. Coefficient is not constant.
f. Not homogenous.
g. Linear, homogeneous, constant coefficient, and degree of 7.

4\. Solve these recurrence relations together with the initial conditions given.
a. $a_n = a_{n-1} + 6a_{n-2}$, for $n \geq 2, a_0 = 3, a_1 = 6$
>Solution
The degree is $2$. Characteristic equation is $r^2-r-6=0$. Its roots are $r=3, -2$.
$$
\begin{aligned}
a_n &= c_1(3)^n + c_2(-2)^n\\
a_0 &= c_1 + c_2 = 3\\
a_1 &= 3c_1 - 2c_2 = 6\\
&\To c_1 = \frac{12}{5}, c_2= \frac{3}{5}\\
a_n &= \frac{12}{5} \cdot 3^n + \frac{3}{5} \cdot (-2)^n
\end{aligned}
$$

d. $a_n = 2a_{n-1} - a_{n-2}$, for $n \geq 2, a_0 = 4, a_1 = 1$
>Solution
The degree is $2$. Characteristic equation is $r^2-2r+1=0$. Its only root is $r=1$.
$$
\begin{aligned}
a_n &= c_1 (1)^n + c_2 \cdot n(1)^n\\
a_0 &= c_1 = 4\\
a_1 &= c_1 + c_2 = 1\\
&\To c_1=4, c_2=-3\\
a_n &= 4 - 3n
\end{aligned}
$$


e. $a_n = a_{n-2}$, for $n \geq 2, a_0 = 5, a_1 = -1$
>Solution
The degree is $2$. Characteristic equation is $r^2-1=0$. Its roots are $r=1, -1$.
$$
\begin{aligned}
a_n &= c_1 (1)^n + c_2 (-1)^n\\
a_0 &= c_1 + c_2 = 5\\
a_1 &= c_1 - c_2 = -1\\
&\To c_1=2, c_2=3\\
a_n &= 2 + 3 \cdot (-1)^n
\end{aligned}
$$

f. $a_n = -6a_{n-1} - 9a_{n-2}$, for $n \geq 2, a_0 = 3, a_1 = -3$
>Solution
The degree is $2$. Characteristic equation is $r^2 + 6r + 9=0$. Its only root is $r=-3$.
$$
\begin{aligned}
a_n &= c_1 (-3)^n + c_2 \cdot n(-3)^n\\
a_0 &= c_1 = 3\\
a_1 &= -3c_1 - 3c_2 = -3\\
&\To c_1=3, c_2=-2\\
a_n &= 3\cdot (-3)^n - 2n \cdot (-3)^n
\end{aligned}
$$

g. $a_{n+2} = -4a_{n+1} + 5a_n$, for $n \geq 0, a_0 = 2, a_1 = 8$
>Solution
The degree is $2$. Characteristic equation is $r^2 + 4r-5=0$. Its roots are $r=1, -5$.
$$
\begin{aligned}
a_n &= c_1 (1)^n + c_2 (-5)^n\\
a_0 &= c_1 + c_2 = 2\\
a_1 &= c_1 - 5c_2 = 8\\
&\To c_1=3, c_2=-1\\
a_n &= 3 - (-5)^n
\end{aligned}
$$

8\. A model for the number of lobsters caught per year is based on the assumption that the number of lobsters caught in a year is the average of the number caught in the two previous years.
a. Find a recurrence relation for $\{L_n\}$, where $L_n$ is the number of lobsters caught in year $n$, under the assumption for this model.
b. Find $L_n$ if $100,000$ lobsters were caught in year $1$ and $300,000$ were caught in year $2$.

>Solution
$$
\begin{aligned}
L_n &= \frac{L_{n-1}}{2} + \frac{L_{n-2}}{2} &\text{ for } n\geq 3\\
L_1 &= 100000 \quad L_2= 300000\\
\end{aligned}
$$
The degree is 2. Characteristic equation is $r^2-\frac{1}{2}r-\frac{1}{2}=0$. Its roots are $r=1, -\frac{1}{2}$.
$$
\begin{aligned}
L_n &= c_1 (1)^n + c_2 (-\frac{1}{2})^n\\
L_1 &= c_1 - \frac{1}{2}c_2 = 100000\\
L_2 &= c_1 + \frac{1}{4}c_2 = 300000\\
&\To c_1=\frac{700000}{3}, c_2=\frac{800000}{3}\\
L_n &= \frac{700000}{3} + \frac{800000}{3} \cdot (-\frac{1}{2})^n
\end{aligned}
$$

12\. Find the solution to $a_n = 2a_{n-1} + a_{n-2} - 2a_{n-3}$ for $n = 3, 4, 5 \cdots$, with $a_0 = 3, a_1 = 6$, and $a_2 = 0$.
>Solution
The degree is 3. Characteristic equation is $r^3 - 2r^2 -r + 2=0$. Its roots are $r=1, 2, -1$.
$$
\begin{aligned}
a_n &= c_1 (1)^n + c_2 (2)^n + c_3 (-1)^n\\
a_0 &= c_1 + c_2 +c_3 = 3\\
a_1 &= c_1 + 2c_2 -c_3 = 6\\
a_2 &= c_1 + 4c_2 +c_3 = 0\\
&\To c_1=6, c_2=-1, c_3=-2\\
a_n &= 6-2^n - 2(-1)^n
\end{aligned}
$$

14\. Find the solution to $a_n = 5a_{n-2} - 4a_{n-4}$ with $a_0 = 3, a_1 = 2, a_2 = 6$, and $a_3 = 8$.
>Solution
The degree is 4. Characteristic equation is $r^4 - 5r^2 + 4=0$. Its roots are $r=1, -1, 2, -2$.
$$
\begin{aligned}
a_n &= c_1 (1)^n + c_2 (-1)^n + c_3 (2)^n + c_4 (-2)^n\\
a_0 &= c_1 + c_2 + c_3 + c_4 = 3\\
a_1 &= c_1 - c_2 + 2c_3 - 2c_4 = 2\\
a_2 &= c_1 + c_2 + 4c_3 + 4c_4 = 6\\
a_3 &= c_1 - c_2 + 8c_3 - 8c_4 = 8\\
&\To c_1=1, c_2=1, c_3=1, c_4=0\\
a_n &= 1 + (-1)^n + 2^n
\end{aligned}
$$
