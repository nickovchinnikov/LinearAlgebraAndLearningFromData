# \#1

#### Example 
$Ax=0$ in $R^4$

$$
\begin{bmatrix}
 1 & 2 & 5 \\
 1 & 2 & 5 \\
 1 & 2 & 5 \\
 1 & 2 & 5 \\
\end{bmatrix}
\cdot 
\begin{bmatrix}
 1 \\
 2 \\
 -1
\end{bmatrix}
=
\begin{bmatrix}
 0 \\
 0 \\
 0 \\
 0
\end{bmatrix}
$$

Dimension: $(4 \times 3)\cdot(3 \times 1)=(4 \times 1)$

$u+v-(u+v)=0$

#### So, any

$$
\begin{bmatrix}
 u & v & u + v
\end{bmatrix}
\cdot
\begin{bmatrix}
 1 \\
 1 \\
 -1
\end{bmatrix}
=
0
$$

#### In the Example
$$
\begin{bmatrix}
 u & v & u + 2v
\end{bmatrix}
\cdot
\begin{bmatrix}
 1 \\
 2 \\
 -1
\end{bmatrix}
=
u + 2v - (u + 2v) = 0
$$

# \# 2

#### Example of $Ax=Ay$

$$
A=\begin{bmatrix}
 u & v & u + v
\end{bmatrix}
$$

$$
A\cdot\begin{bmatrix}
 1 \\
 1 \\
 -1
\end{bmatrix}
=
A\cdot\begin{bmatrix}
 -1 \\
 -1 \\
 1
\end{bmatrix}
\implies
u + v - (u+v) = -u - v + (u+v)
$$

$Az = 0$

$$
\begin{bmatrix}
 u & v
\end{bmatrix}
\cdot
z=0
\implies
z_1 \cdot u + z_2 \cdot v = 0
$$

#### So

$z = 0$

#### Or

$z = \begin{bmatrix}
 -v \\
 u
\end{bmatrix}$

#### Or

$z = \begin{bmatrix}
 v \\
 -u
\end{bmatrix}$

# \# 3

The vectors $a_1, a_2, \dots, a_n$ in $R^m$ and $c_1 \cdot a_1 + \dots + c_n \cdot a_n = 0$

#### Matrix notation
$$
\begin{bmatrix}
  |  &  |  &        &  |  \\
 a_1 & a_2 & \cdots & a_n \\
  |  &  |  &        &  |  \\
\end{bmatrix}
\cdot
\begin{bmatrix}
 c_1 \\
 c_2 \\
 \vdots \\
 c_n
\end{bmatrix}
=
0
$$
#### Or

$$
\begin{bmatrix}
 a_{11} & a_{12} & \cdots & a_{1n} \\
 a_{21} & a_{22} & \cdots & a_{2n} \\
 \vdots & \vdots & \ddots & \vdots\\
 a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}
\cdot
\begin{bmatrix}
 c_1 \\
 c_2 \\
 \vdots \\
 c_n
\end{bmatrix}
=
c_{1}
\cdot
\begin{bmatrix}
 a_{11} \\
 a_{12} \\
 \vdots \\
 a_{1n}
\end{bmatrix}
+
\cdots
+
c_{n}
\cdot
\begin{bmatrix}
 a_{m1} \\
 a_{m2} \\
 \vdots \\
 a_{mn}
\end{bmatrix}
=
0
$$

#### Sigma notation
$$
\sum_{i=1}^{m} \sum_{j=1}^{n} a_{ij} * c_{j} = 0
$$

# \# 4




```python

```
