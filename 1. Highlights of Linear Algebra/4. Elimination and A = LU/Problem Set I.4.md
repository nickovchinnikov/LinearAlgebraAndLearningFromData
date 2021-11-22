# Problem Set I.4

## 1. Factor matrices into A = LU

### Matrix 1

$
A=\begin{bmatrix}
 2 & 1 \\
 6 & 7
\end{bmatrix}
$;

#### Step 1

$
l_{11}=1
$

$
l_{21}=\frac{a_{21}}{a_{11}}=\frac{6}{2}=3
$;

$u_1=$ first row of A = $\begin{bmatrix}2 & 1\end{bmatrix}$

So,

$l_{1}=\begin{bmatrix}
 1 \\
 3
\end{bmatrix}$

And 

$l_{1} \cdot u_{1}^{*} = 
\begin{bmatrix}
 1 \\
 3
\end{bmatrix} 
\cdot 
\begin{bmatrix}
 2 & 1
\end{bmatrix} =
\begin{bmatrix}
 2 & 1 \\
 6 & 3
\end{bmatrix}
$

#### Step 2

$$A - l_{1} \cdot u_{1}^{*} = 
\begin{bmatrix}
 2 & 1 \\
 6 & 7
\end{bmatrix}
- 
\begin{bmatrix}
 2 & 1 \\
 6 & 3
\end{bmatrix}
=
\begin{bmatrix}
 0 & 0 \\
 0 & 4
\end{bmatrix}
$$

$A_{2}=
\begin{bmatrix}
  4
\end{bmatrix}$


So,

$l_{2} = \begin{bmatrix}
  0 \\
  1
\end{bmatrix}
$ <- last col

And

$u_{2}=\begin{bmatrix}
  0 & 4
\end{bmatrix}$ <- result of elimination

$
l_{2} \cdot u_{2}^* = \begin{bmatrix}
  0 & 0 \\
  0 & 4
\end{bmatrix}
$

#### Result

$$A = l_{1} \cdot u_{1}^{*} + l_{2} \cdot u_{2}^{*} = 
\begin{bmatrix}
 2 & 1 \\
 6 & 3
\end{bmatrix}
+
\begin{bmatrix}
  0 & 0 \\
  0 & 4
\end{bmatrix}
=
\begin{bmatrix}
 2 & 1 \\
 6 & 7
\end{bmatrix}
$$

And

$$A=
\begin{bmatrix}
 l_{1} & l_{2}
\end{bmatrix}
\cdot
\begin{bmatrix}
 u_{1}^* \\
 u_{2}^*
\end{bmatrix}
=
\begin{bmatrix}
 1 & 0 \\
 3 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
 2 & 1 \\
 0 & 4
\end{bmatrix}
=
\begin{bmatrix}
 2 & 1 \\
 6 & 7
\end{bmatrix}
$$

### Matrix 2

$A=\begin{bmatrix}
 1 & 1 & 1 \\
 1 & 1 & 1 \\
 1 & 1 & 1
\end{bmatrix}$

#### Step 1:

$
l_{11}=1
$,

$
l_{21}=\frac{a_{21}}{a_{11}}=\frac{1}{1}=1
$,

$
l_{31}=\frac{a_{31}}{a_{11}}=\frac{1}{1}=1
$;

$u_1=$ first row of A = $\begin{bmatrix}
 1 & 1 & 1
\end{bmatrix}$

So,

$l_{1} \cdot u_{1}^* = \begin{bmatrix}
 1 \\
 1 \\
 1
\end{bmatrix}
\cdot
\begin{bmatrix}
 1 & 1 & 1
\end{bmatrix}
$

#### Step 2

$$
A - l_{1} \cdot u_{1}^{*} = 
\begin{bmatrix}
 1 & 1 & 1 \\
 1 & 1 & 1 \\
 1 & 1 & 1
\end{bmatrix}
- 
\begin{bmatrix}
 1 & 1 & 1 \\
 1 & 1 & 1 \\
 1 & 1 & 1
\end{bmatrix}
=
\begin{bmatrix}
 0 & 0 & 0 \\
 0 & 0 & 0 \\
 0 & 0 & 0
\end{bmatrix} = A_{2}
$$

So,

$$l_{2} = \begin{bmatrix}
 0 \\
 1 \\
 1
\end{bmatrix}$$

and

$$l_{3} = \begin{bmatrix}
 0 \\
 0 \\
 1
\end{bmatrix}$$

#### Result

$$
A
=
LU
=
\begin{bmatrix}
 1 & 0 & 0 \\
 1 & 1 & 0 \\
 1 & 1 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
 1 & 1 & 1 \\
 0 & 0 & 0 \\
 0 & 0 & 0
\end{bmatrix}
$$

### Matrix 3

$$
A=\begin{bmatrix}
  2 & -1 &  0 \\
 -1 &  2 & -1 \\
  0 & -1 &  2
\end{bmatrix}
$$

#### Step 1


$
l_{11}=1
$,

$
l_{21}=\frac{a_{21}}{a_{11}}=\frac{-1}{2}
$,

$
l_{31}=\frac{a_{31}}{a_{11}}=\frac{0}{2} = 0
$;

$u_1=$ first row of A = $\begin{bmatrix} 2 & -1 & 0 \end{bmatrix}$

And 

$$l_{1} \cdot u_{1}^{*} = 
\begin{bmatrix}
 1            \\
 \frac{-1}{2} \\
 0
\end{bmatrix} 
\cdot 
\begin{bmatrix}
 2 & -1 & 0
\end{bmatrix} =
\begin{bmatrix}
  2 &      -1     & 0 \\
 -1 & \frac{1}{2} & 0 \\
  0 &       0     & 0
\end{bmatrix}
$$

#### Step 2

$$
A - l_{1} \cdot u_{1}^{*} = 
\begin{bmatrix}
  2 & -1 &  0 \\
 -1 &  2 & -1 \\
  0 & -1 &  2
\end{bmatrix}
- 
\begin{bmatrix}
  2 &      -1     & 0 \\
 -1 & \frac{1}{2} & 0 \\
  0 &       0     & 0
\end{bmatrix}
=
\begin{bmatrix}
 0 &       0      &  0 \\
 0 & \frac{3}{2}  & -1 \\
 0 &      -1      &  2
\end{bmatrix};
A_{2}=\begin{bmatrix}
 \frac{3}{2}  & -1 \\
      -1      &  2
\end{bmatrix}
$$

#### Rest of the data
$$
\begin{bmatrix}
    -  & u_1^*  & -  \\
  \begin{matrix}
    0 \\
    0
  \end{matrix}  & {A_2}
\end{bmatrix}
=
\begin{bmatrix}
 2 &      -1      &  0 \\
 0 & \frac{3}{2}  & -1 \\
 0 &      -1      &  2
\end{bmatrix}
$$

$$
l_{21}=0,
l_{22}=1,
l_{23}=\frac{a_{32}}{a_{22}}=\frac{-1}{\frac{3}{2}} = -\frac{2}{3}$$

$u_2=$ (second row of the rest) = $\begin{bmatrix} 0 & \frac{3}{2} & -1 \end{bmatrix}$

And 

$$l_{2} \cdot u_{2}^{*} = 
\begin{bmatrix}
 0  \\
 1 \\
 -\frac{2}{3}
\end{bmatrix} 
\cdot 
\begin{bmatrix} 0 & \frac{3}{2} & -1 \end{bmatrix}
=
\begin{bmatrix}
  0 &        0     &        0     \\
  0 &  \frac{3}{2} &       -1     \\
  0 &       -1     &   \frac{2}{3}
\end{bmatrix}
$$

$$
A - l_{1} \cdot u_{1}^{*} - l_{2} \cdot u_{2}^{*} = 
\begin{bmatrix}
 0 &       0      &  0 \\
 0 & \frac{3}{2}  & -1 \\
 0 &      -1      &  2
\end{bmatrix}
-
\begin{bmatrix}
  0 &        0     &        0     \\
  0 &  \frac{3}{2} &       -1     \\
  0 &       -1     &   \frac{2}{3}
\end{bmatrix}
=
\begin{bmatrix}
  0 &        0     &        0     \\
  0 &        0     &        0     \\
  0 &        0     &   \frac{4}{3}
\end{bmatrix}
= A_3
$$

$
l_{31}=0
$,

$
l_{32}=0
$,

$
l_{33}=1
$;

$$u_3=\begin{bmatrix}
  0 \\        0     \\   \frac{4}{3}
\end{bmatrix}$$

#### Result

$$
A=LU=
\begin{bmatrix}
        1     &        0     &   0 \\
 -\frac{1}{2} &        1     &   0 \\
        0 &     -\frac{2}{3} &   1
\end{bmatrix}
\cdot
\begin{bmatrix}
  2 &       -1     &        0 \\
  0 &  \frac{3}{2} &       -1 \\
  0 &        0     &  \frac{4}{3}
\end{bmatrix}
=
\begin{bmatrix}
  2 & -1 &  0 \\
 -1 &  2 & -1 \\
  0 & -1 &  2
\end{bmatrix}
$$

## 2. Find a formula
for the $a_{ij}$ to a rank 1 matrix 

Rank 1 matrix

$$
\begin{bmatrix}
  a_{11} &  a_{12} &  \cdots & a_{1n} \\
  a_{21} &  a_{22} &  \cdots & a_{2n} \\
  \vdots &  \cdots &  \ddots & \vdots \\
  a_{m1} &  a_{m2} &  \cdots & a_{mn}
\end{bmatrix}
$$

$$
A = LU = l_{1} \cdot u_{1}^* + \cdots + l_{n} \cdot u_{n}^* = 
\begin{bmatrix}
  l_1 & \cdots & l_n
\end{bmatrix}
\cdot
\begin{bmatrix}
  u_1^*  \\
  \vdots \\
  u_n^*
\end{bmatrix}
$$

And

$l_{11} = 1$, $l_{21} = \frac{a_{21}}{a_{11}}$, $l_{31} = \frac{a_{31}}{a_{11}}$, ... ,$l_{m1} = \frac{a_{m1}}{a_{11}}$

$a_{ij}=\frac{a_{j1} \cdot u_{1j}}{a_{11}}$

So, when $a_{11} = 0$ this formula breaks down!

## 3. Find a matrix

$EA=U$, what is $E$?

$A=LU,L^{-1}A=U,E=L^{-1} \implies E^{-1}=(L^{-1})^{-1}=L$

$$
A=\begin{bmatrix}
  2 &  1 &  0 \\
  0 &  4 &  2 \\
  6 &  3 &  5
\end{bmatrix}
$$

### Step 1

$l_{11}=1,l_{21}=\frac{a_{21}}{a_{11}}=l_{21}=\frac{0}{2}=0,l_{31}=\frac{a_{31}}{a_{11}}=\frac{6}{2}=3$

$$l_1=\begin{bmatrix}
1 \\
0 \\
3
\end{bmatrix}$$

$ u_1^* = $ first row of $A = \begin{bmatrix} 2 & 1 & 0 \end{bmatrix} $

$$ l_{1} \cdot u_1^* = \begin{bmatrix}
  1 \\
  0 \\
  3
\end{bmatrix} \cdot \begin{bmatrix} 2 & 1 & 0 \end{bmatrix}
=
\begin{bmatrix}
  2 & 1 & 0 \\
  0 & 0 & 0 \\
  6 & 3 & 0
\end{bmatrix}
$$

$$A - l_{1} \cdot u_1^* = 
\begin{bmatrix}
  2 &  1 &  0 \\
  0 &  4 &  2 \\
  6 &  3 &  5
\end{bmatrix}
-
\begin{bmatrix}
  2 & 1 & 0 \\
  0 & 0 & 0 \\
  6 & 3 & 0
\end{bmatrix}
=
\begin{bmatrix}
  0 & 0 & 0 \\
  0 & 4 & 2 \\
  0 & 0 & 5
\end{bmatrix}
=
\begin{bmatrix}
 4 & 2 \\
 0 & 5
\end{bmatrix}
=
A_2
$$

#### Rest of the data

$$\begin{bmatrix}
    -  & u_1^*  & -  \\
  \begin{matrix}
    0 \\
    0
  \end{matrix}  & {A_2}
\end{bmatrix}
=
\begin{bmatrix}
 2 &      1      &  0 \\
 0 &      4      &  2 \\
 0 &      0      &  5
\end{bmatrix}$$

### Step 2



$l_{12}=0,l_{22}=1,l_{23}=\frac{a_{32}}{a_{22}}=\frac{0}{4}=0$

$$l_2=\begin{bmatrix}
0 \\
1 \\
0
\end{bmatrix}$$

$u_2^{*} = $ second row of $A = \begin{bmatrix} 0 & 4 & 2 \end{bmatrix} $

$$l_2 \cdot u_2^{*} = \begin{bmatrix}
  0 & 0 & 0 \\
  0 & 4 & 2 \\
  0 & 0 & 0
\end{bmatrix}$$

$$A - l_{1} \cdot u_1^* - l_2 \cdot u_2^{*} = \begin{bmatrix}
    -  & u_1^*  & -  \\
  \begin{matrix}
    0 \\
    0
  \end{matrix}  & {A_2}
\end{bmatrix}
-
\begin{bmatrix}
  0 & 0 & 0 \\
  0 & 4 & 2 \\
  0 & 0 & 0
\end{bmatrix}
=
\begin{bmatrix}
  0 & 0 & 0 \\
  0 & 0 & 0 \\
  0 & 0 & 5
\end{bmatrix}
=
\begin{bmatrix}
  5
\end{bmatrix}
=
A_3
$$

### Step 3

$$l_3=\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}$$

$$u_3^*=\begin{bmatrix}
  0 & 0 & 5
\end{bmatrix}$$

$$l_3 \cdot u_3^* = \begin{bmatrix}
  0 & 0 & 0 \\
  0 & 0 & 0 \\
  0 & 0 & 5
\end{bmatrix}$$

$ A = l_{1} \cdot u_1^* + l_2 \cdot u_2^{*} + l_3 \cdot u_3^* = \begin{bmatrix}
  2 &  1 &  0 \\
  0 &  4 &  2 \\
  6 &  3 &  5
\end{bmatrix} $

$A=LU=\begin{bmatrix}
  1 & 0 & 0 \\
  0 & 1 & 0 \\
  3 & 0 & 1
\end{bmatrix} \cdot \begin{bmatrix}
  2 & 1 & 0 \\
  0 & 4 & 2 \\
  0 & 0 & 5
\end{bmatrix}$

$L^{-1} = \begin{bmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
  -3 & 0 & 1
\end{bmatrix}$

$L^{-1}A = \begin{bmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
  -3 & 0 & 1
\end{bmatrix} \cdot
\begin{bmatrix}
  2 &  1 &  0 \\
  0 &  4 &  2 \\
  6 &  3 &  5
\end{bmatrix} =
\begin{bmatrix}
  2 & 1 & 0 \\
  0 & 4 & 2 \\
  0 & 0 & 5
\end{bmatrix}$

## 4. How the one-step inverses multiply to give L

$$A=\begin{bmatrix}
  1 & 0 & 0 \\
  a & 1 & 0 \\
  b & c & 1
\end{bmatrix}$$

$$
E_1=\begin{bmatrix}
   1 & 0 & 0 \\
  -a & 1 & 0 \\
  -b & 0 & 1
\end{bmatrix}
$$

$$
E_2=\begin{bmatrix}
  1 &  0 & 0 \\
  0 &  1 & 0 \\
  0 & -c & 1
\end{bmatrix}
$$

$$
E = E_2E_1 =
\begin{bmatrix}
  1 &  0 & 0 \\
  0 &  1 & 0 \\
  0 & -c & 1
\end{bmatrix}\begin{bmatrix}
   1 & 0 & 0 \\
  -a & 1 & 0 \\
  -b & 0 & 1
\end{bmatrix}
=
\begin{bmatrix}
     1   &  0 & 0 \\
    -a   &  1 & 0 \\
  ac - b & -c & 1
\end{bmatrix} = A^{-1}
$$

$$EA=I$$

$$\begin{bmatrix}
     1   &  0 & 0 \\
    -a   &  1 & 0 \\
  ac - b & -c & 1
\end{bmatrix}\begin{bmatrix}
  1 & 0 & 0 \\
  a & 1 & 0 \\
  b & c & 1
\end{bmatrix}
=
\begin{bmatrix}
  1 & 0 & 0 \\
  0 & 1 & 0 \\
  0 & 0 & 1
\end{bmatrix}$$

$$\begin{vmatrix}
   1 & 0 & 0 \\
  -a & 1 & 0 \\
  -b & 0 & 1
\end{vmatrix}\begin{vmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
   0 & 0 & 1
\end{vmatrix}
\begin{matrix}
   \\
   row_{2} + a \cdot row_{1} & \implies & row_{2} \\
   row_{3} + b \cdot row_{1} & \implies & row_{3}
\end{matrix}
=
\begin{vmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
   0 & 0 & 1
\end{vmatrix}\begin{vmatrix}
   1 & 0 & 0 \\
   a & 1 & 0 \\
   b & 0 & 1
\end{vmatrix}=E_1^{-1}
$$

$$\begin{vmatrix}
   1 &  0 & 0 \\
   0 &  1 & 0 \\
   0 & -c & 1
\end{vmatrix}\begin{vmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
   0 & 0 & 1
\end{vmatrix}
\begin{matrix}
   \\
   \\
   row_{3} + c \cdot row_{2} & \implies & row_{3}
\end{matrix}
=
\begin{vmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
   0 & 0 & 1
\end{vmatrix}\begin{vmatrix}
   1 &  0 & 0 \\
   0 &  1 & 0 \\
   0 &  c & 1
\end{vmatrix}=E_2^{-1}
$$

$$
E_1^{-1}E_2^{-1}=\begin{bmatrix}
   1 & 0 & 0 \\
   a & 1 & 0 \\
   b & 0 & 1
\end{bmatrix}\begin{bmatrix}
   1 &  0 & 0 \\
   0 &  1 & 0 \\
   0 &  c & 1
\end{bmatrix}
=
\begin{bmatrix}
   1 &  0 & 0 \\
   a &  1 & 0 \\
   b &  c & 1
\end{bmatrix}=A
$$

## 5. When A=LU is not possible

#### 5.1. A=LU

$$
\begin{bmatrix}
   0 & 1 \\
   2 & 3
\end{bmatrix}=
\begin{bmatrix}
   1 & 0 \\
   l & 1
\end{bmatrix}
\begin{bmatrix}
   d & e \\
   0 & f
\end{bmatrix}
$$

$$
\begin{bmatrix}
   1 & 0
\end{bmatrix}
\begin{bmatrix}
   d \\
   0
\end{bmatrix}=0,d=0
$$

#### impossible!
$$
\begin{bmatrix}
   l & 1
\end{bmatrix}
\begin{bmatrix}
   d \\
   0
\end{bmatrix}=2,l \cdot d=2
$$

#### 5.2. A = LU

$$
\begin{bmatrix}
   1 & 1 & 0 \\
   1 & 1 & 2 \\
   1 & 2 & 1
\end{bmatrix}=
\begin{bmatrix}
   1 & 0 & 0 \\
   l & 1 & 0 \\
   m & n & 1
\end{bmatrix}
\begin{bmatrix}
   d & e & g \\
   0 & f & h \\
   0 & 0 & i
\end{bmatrix}
$$

$$
LU = \begin{bmatrix}
   1 & 0 & 0 \\
   1 & 1 & 0 \\
   1 & n & 1
\end{bmatrix}
\begin{bmatrix}
   1 & 1 & 0 \\
   0 & 0 & 2 \\
   0 & 0 & i
\end{bmatrix}
$$

$
a_{32}=2
$, so
$
\begin{bmatrix}
   1 & n & 1
\end{bmatrix}
\begin{bmatrix}
   1 \\
   0 \\
   0
\end{bmatrix}=1 + 0 \cdot n + 0 \neq 2
$, impossible!

## 6.

$$A=\begin{bmatrix}
   1 & c & 0 \\
   2 & 4 & 1 \\
   3 & 5 & 1
\end{bmatrix}$$

When $c=2$, $a_{22}=0$, because $row_1$ and $row_2$ are dependent in this case

$$\begin{bmatrix}
   1 & 2 & 0 \\
   2 & 4 & 1 \\
   3 & 5 & 1
\end{bmatrix}
\begin{matrix}
   \\
   row_{2} - 2 \cdot row_{1} & \implies & row_{2} \\
\end{matrix}
=
\begin{vmatrix}
   1 & 2 & 0 \\
   0 & 0 & 1 \\
   3 & 5 & 1
\end{vmatrix}$$

second pivot is zero

When $c=1$

$$\begin{bmatrix}
   1 & 1 & 0 \\
   2 & 4 & 1 \\
   3 & 5 & 1
\end{bmatrix}
\begin{matrix}
   \\
   row_{2} - 2 \cdot row_{1} & \implies & row_{2} \\
   row_{3} - 3 \cdot row_{1} & \implies & row_{3}
\end{matrix}
=
\begin{bmatrix}
   1 & 1 & 0 \\
   0 & 2 & 1 \\
   0 & 2 & 1
\end{bmatrix}$$

$row_2$ and $row_3$ are dependent in this case, so 3'rd pivot is zero!

## 7. L and U for symmetric matrix A

$$A=\begin{bmatrix}
   a & a & a & a \\
   a & b & b & b \\
   a & b & c & c \\
   a & b & c & d
\end{bmatrix}
$$

$$A=\begin{bmatrix}
   a & a & a & a \\
   a & b & b & b \\
   a & b & c & c \\
   a & b & c & d
\end{bmatrix}=LU=
\begin{bmatrix}
   1 & 0 & 0 & 0 \\
   1 & 1 & 0 & 0 \\
   1 & 1 & 1 & 0 \\
   1 & 1 & 1 & 1
\end{bmatrix}\begin{bmatrix}
   a & a   & a   & a \\
   0 & b-a & b-a & b-a \\
   0 & 0   & c-b & c-b \\
   0 & 0   & 0   & d-c
\end{bmatrix}$$

## 8. Tridiagonal matrices

$$A=\begin{bmatrix}
   1 & 1 & 0 \\
   1 & 2 & 1 \\
   0 & 1 & 2
\end{bmatrix}
$$

Symmetry produces

$$A=LU=\begin{bmatrix}
   1 & 0 & 0 \\
   1 & 1 & 0 \\
   0 & 1 & 1
\end{bmatrix}\begin{bmatrix}
   1 & 1 & 0 \\
   0 & 1 & 1 \\
   0 & 0 & 1
\end{bmatrix}=LL^{T}
$$

$$LDL^{T}=\begin{bmatrix}
   1 & 0 & 0 \\
   1 & 1 & 0 \\
   0 & 1 & 1
\end{bmatrix}\begin{bmatrix}
   1 & 0 & 0 \\
   0 & 1 & 0 \\
   0 & 0 & 1
\end{bmatrix}\begin{bmatrix}
   1 & 1 & 0 \\
   0 & 1 & 1 \\
   0 & 0 & 1
\end{bmatrix}$$

$$A=\begin{bmatrix}
   a & a   & 0 \\
   a & a+b & b \\
   0 & b   & b+c
\end{bmatrix}
$$

$$LDL^{T}=\begin{bmatrix}
   1 & 0 & 0 \\
   1 & 1 & 0 \\
   0 & 1 & 1
\end{bmatrix}\begin{bmatrix}
   a & 0 & 0 \\
   0 & b & 0 \\
   0 & 0 & c
\end{bmatrix}\begin{bmatrix}
   1 & 1 & 0 \\
   0 & 1 & 1 \\
   0 & 0 & 1
\end{bmatrix}
=
\begin{bmatrix}
   a & 0 & 0 \\
   a & b & 0 \\
   0 & b & c
\end{bmatrix}\begin{bmatrix}
   1 & 1 & 0 \\
   0 & 1 & 1 \\
   0 & 0 & 1
\end{bmatrix}
=
\begin{bmatrix}
   a & a   & 0 \\
   a & a+b & b \\
   0 & b   & b+c
\end{bmatrix}$$

## 9. Pivots

$$A=\begin{bmatrix}
   5 &     &  \\
     &  9  &  \\
     &     & 3
\end{bmatrix}
$$
$$A_2=\begin{bmatrix}
   5 &  \\
     & 9 
\end{bmatrix}$$

## 10. Look at each of the square upper left submatrices

$$A_k=L_kU_k=\begin{bmatrix}
   L_k &  0  \\
   *   &  *
\end{bmatrix}\begin{bmatrix}
   U_k &  *  \\
   0   &  *
\end{bmatrix}$$

## 11. The first pivot is the largest number

$$A=\begin{bmatrix}
   1 & 2  \\
   3 & [4]
\end{bmatrix}$$
The largest $|a_{ij}|=4$, first pivot columns $\begin{bmatrix}
   2  \\
   4
\end{bmatrix}$$

$$\frac{1}{|a_{ij}|} \cdot col_j =
\frac{1}{4} \cdot \begin{bmatrix}
   2  \\
   4
\end{bmatrix} =
\begin{bmatrix}
   1/2  \\
   1
\end{bmatrix}$$

$$l_1u_1^*=\begin{bmatrix}
   1/2  \\
   1
\end{bmatrix} \cdot \begin{bmatrix}
   3  & 4
\end{bmatrix}=\begin{bmatrix}
   3/2 & 2  \\
   3   & 4
\end{bmatrix}$$

$$A-l_1u_1^*=\begin{bmatrix}
   -1/2 & 0  \\
   0    & 0
\end{bmatrix}$$

$$\begin{bmatrix}
   1/2  \\
   1
\end{bmatrix} \cdot \begin{bmatrix}
   3  & 4
\end{bmatrix}+\begin{bmatrix}
   -1/2 & 0  \\
   0    & 0
\end{bmatrix}=l_1u_1^*+l_2u_2^*=\begin{bmatrix}
   1/2 & 1  \\
   1   & 0
\end{bmatrix}\begin{bmatrix}
   3      & 4  \\
   -1/2   & 0
\end{bmatrix}$$

$$P_1AP_2=LU,P_1AP_2=\begin{bmatrix}
   1   & 0 \\
   1/2 & 1
\end{bmatrix}\begin{bmatrix}
   4 & 3  \\
   0 & -1/2
\end{bmatrix}=\begin{bmatrix}
   4 & 3 \\
   2 & 1
\end{bmatrix}=A$$

$$P_1AP_2=\begin{bmatrix}
   0 & 1 \\
   1 & 0
\end{bmatrix}\begin{bmatrix}
   1 & 2  \\
   3 & 4
\end{bmatrix}\begin{bmatrix}
   0 & 1 \\
   1 & 0
\end{bmatrix}=\begin{bmatrix}
   4 & 3 \\
   2 & 1
\end{bmatrix}$$

$$P_1L=\begin{bmatrix}
   0 & 1 \\
   1 & 0
\end{bmatrix}\begin{bmatrix}
   1   & 0  \\
   1/2 & 1
\end{bmatrix}=\begin{bmatrix}
   1/2 & 1 \\
   1   & 0
\end{bmatrix}$$

$$UP_2=\begin{bmatrix}
   4 &  3  \\
   0 & -1/2
\end{bmatrix}\begin{bmatrix}
   0 & 1 \\
   1 & 0
\end{bmatrix}=\begin{bmatrix}
    3   & 4 \\
   -1/2 & 0
\end{bmatrix}$$

$$P_1LUP_2=\begin{bmatrix}
   1/2 & 1 \\
   1   & 0
\end{bmatrix}\begin{bmatrix}
    3   & 4 \\
   -1/2 & 0
\end{bmatrix}=\begin{bmatrix}
   1 & 2  \\
   3 & 4
\end{bmatrix}=A$$


```python

```
