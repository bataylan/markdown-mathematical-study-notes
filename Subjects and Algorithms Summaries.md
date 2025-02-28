\require{AMSmath}
\require{AMSsymbols}
# Subjects and Algorithms Summaries

## Limit
#### Existance
Limit exists $\iff$ left-hand and right-hand limits exists and
$\lim\limits_{x \to a^-}f(x) = \lim\limits_{x \to a^+}f(x)$.

## Functions

#### Monotonic Functions
If function f is increasing ($f'(x)>0$) or decreasing ($f'(x)<0$) for an interval
$\Rightarrow$ f is Monotonic function.

#### Solving Inverse  of a Functions
1)Solve $y=f(x)$ for x
$$ x = f^{-1}(y) $$

2)Interchange x and y to obtain

$$ y = f^{-1}(x) $$

#### Continuity
$f(x)$ is continous $\iff$ followings holds:
$$ 1) \exists f(c) \quad (c\in D(f)) $$
$$ 2) \exists \lim\limits_{x \to c}f(x) $$
$$ 3) \lim\limits_{x \to 0}f(x) = f(c) $$
(Function is continous $\iff$ there exists $f(c)$ and limit exists at c and
limit of f(x) at when x $\to$ c is equalt to $f(c)$).

## One-variable Calculus

#### Vertical Asymptote
If
$$ \lim\limits_{x \to a^+}f(x) = \pm \infty \quad \lor \quad \lim\limits_{x \to a^-}f(x) = \pm \infty$$
a is vertical asymptote.

#### Horizontal Asymptote
If
$$ \lim\limits_{x \to \infty}f(x) = b \quad \lor \quad \lim\limits_{x \to -\infty}f(x) = b$$
horizontal asymptote.

#### Oblique or Slant Asymptote

An oblique or a slant asymptote is an asymptote
that is neither vertical or horizontal.

If the degree of the numerator is one more than
the degree of the denominator, then the graph of
the rational function will have a slant asymptote.
Slant asymptote find by long division of the rational function. When denumerator's
degree is equal to one, numerator is the asymptote function.

!* A graph can have both a vertical and a slant asymptote, but it CANNOT
have both a horizontal and slant asymptote.

#### L'Hospital's Rule
$\underline{\text{!This rule is can be used in only one-variable calculus}}$


If  $\lim\limits_{x \to a}\frac{f(x)}{g(x)} = \frac{0}{0} \lor \frac{\infty}{\infty}$, take
derivates of  numerator and denumerator seperately ($\frac{f'(x)}{g'(x)}$) until
it is $\neq \frac{0}{0}$ or $\frac{\infty}{\infty}$

#### Sandwich Theorem
Suppose $g(x)\leq f(x) \leq h(x)$ and $\lim\limits_{x \to c}g(x) = \lim\limits_{x \to c}h(x) = L$. Then,
$$ \lim\limits_{x \to c}f(x) = L $$

#### Tangent Line to the Curve
Let $y = f(x)$ at $(x_0, y_0)$

1) Calculate slope m: $m=\lim\limits_{h \to 0}\frac{f(x_0+h)-f(x_0)}{h} = f'(x_0)$

2) If limit exists, find tangent line: $y=y_0+m(x-x_0)$

#### Instantaneous Speed
$$ \lim\limits_{\bigtriangleup t \to 0}\frac {\bigtriangleup s}{\bigtriangleup t} = f'(x_0)$$


#### Graphing steps for y=f(x)
1) Identify domain of f and symmetries (even/odd)(horizontal/vertical/slant)

2) Find $y', y''$

3) Find critical points(bounds, $f'(x)=0$, $\nexists f'(x)$) as ($x,y$).

4) Find intervals of f that it is increasing ($f'(x)>0$) or decreasing ($f'(x)<0$)

5) Find local max and minimums (critical points that change signs $f'(x)$).

6) Calculate all critical points and find absolute min and abosulute max.

7) Find points of inflection ($f''(x) = 0$) and concavity ($f''<0$ and $f''>0$)

8) Plot key points, intersections then concavities.

#### Shifting and Strecthing Graph
Let $y=af(b(x+c))+d$.

a: (+) $\to$ horizontal stretch or compression, (-) $\to$ reflection about y-axis

b: (+) $\to$ vertical strecth or compression, (-) $\to$ reflection about x-axis

c: horizontal Shifting

d: vertical shift


##### Rolle's Theorem
Let $f(x)=y$ is continuous at every point of [a,b] and differentiable at every
point of (a,b). Then, if $f(a) = f(b)$ then $\exists c$ that $f'(c)=0$.

#### Mean-Value Theorem
Mean-Value theorem use Rolle's Theorem to get this equation:
$$ \frac{f(b)-f(a)}{b-a}=f'(c) $$



### Integral
#### Integration by Parts
$$ \int (f(x)g'(x))dx = f(x)g(x)-\int (f'(x)g(x))dx $$

Let $u = f(x)$ and $v=g(x)$. Then the statement will be
$$ \int(u)dv = uv - \int (v)du $$

*Priority of picking u is shortened by $\underline{\text{LIATE}}$ (L-Logarithms,
I-Inverse Trigonometric, A-Algebraic, T-Trigonometric, E-Exponential)

#### Taking Integral of Powers of Cosinus and Sinus
Let $\int (\sin^m(x).\cos^n(x))dx$.

1) If m-odd $\to$ replace $\sin^2(x)$ with $\sin^2(x) = 1-\cos^2(x)$

2) If m-even and n-odd $\to$ replace $\cos^2(x)$ with $\cos^2(x) = 1-sin^2(x)$

3) If m-even and n-even $\to$ replace $\sin^2(x)$ with $\sin^2(x) = \frac{1-\cos(2x)}{2}$
and $\cos^2(x) = \frac{1+\cos(2x)}{2}$


## Vector Calculus
##### Area of Parallelogram
$$ ||u \times v|| = |u||v|\sin(\theta) $$

##### Volume of Parallelpiped (Triple Scalar Product)
$$ (u \times v).w = \begin{vmatrix}
u_1 & y_3 & u_3 \\
v_1 & v_2 & v_3 \\
w_1 & w_2 & w_3
 \end{vmatrix} $$

##### Vector Equation for line
 $r_0$ is initial point, t is parameter (scalar), v is direction vector (usually unit vector)
 $$ r(t) = r_0 + tv $$


##### Distance from a Point to a line
![](assets/point-to-line-distance.png =x200)

$$ \frac{|\overrightarrow{PQ} \times \overrightarrow{n}|}{||\overrightarrow{n}||} = distance $$

#### Plane Equation
![](assets/plane-equation.png =x300)

Normal Vector to a plane: $n = Ai + Bj + Ck$

Plane = $n.\overrightarrow{P_0P}$

= $A(x-x_0)+B(y-y_0)+C(z-z_0) = D$

So, the final equation for plane is:

$$ A(x-x_0)+B(y-y_0)+C(z-z_0) - D = 0 $$


#### Line of Intersection of Two Planes

![](assets/intersection-of-two-planes.png =x200)

Let planes $P_1$ and $P_2$ are $P_1=A_1x + B_1y+C_1z = D_1$ and $P_2=A_2x+B_2y+C_2z = D_2$

1) Find an intersection point ($P_0$) of two planes: $P_1 = P_2$

2) Find direction vector ($\overrightarrow{u}$) of intersection line

$$ \overrightarrow{u} = \overrightarrow{n_1} \times \overrightarrow{n_2} =  \begin{vmatrix}
i & j & k \\
A_1 & B_1 & C_1 \\
A_2 & B_2 & C_2
 \end{vmatrix} $$

3) Write new plane equation as follows:
$$ A_3(x-x_0)+B_3(y-y_0)+C_3(z-z_0) - D = 0 $$


##### Distance from a Point to a Plane
![](assets/point-to-plane-distance.png =x250)

$$ \frac{|\overrightarrow{PQ} . \overrightarrow{n}|}{||\overrightarrow{n}||} = distance $$

##### Angle between two vectors

$$ \cos(\theta) = \frac {\overrightarrow{u} .  \overrightarrow{v}}{||\overrightarrow{u}||.||\overrightarrow{v}||}

\Rightarrow \theta = \cos^{-1} \Bigg(
\frac{\overrightarrow{u}.\overrightarrow{v}}{||\overrightarrow{u}||.||\overrightarrow{v}||} \Bigg) $$


##### Angle between two Planes
$$ \theta = \cos^{-1} \Bigg(
\frac{\overrightarrow{n_1}.\overrightarrow{n_2}}{||\overrightarrow{n_1}||.||\overrightarrow{n_2}||} \Bigg) $$


##### Velocity, Speed and Acceleration
Let $c(t) = (x(t), y(t), z(t))$ is path.
$$ c'(t) = v \to \mathrm{velocity} $$
$$ |c'(t)| = |v| \to \mathrm{speed}  $$
$$ a = c''(t) = v' \to \mathrm{acceleration} $$



##### Gradient of f
![](assets/gradient-of-f.png =x300)
$$ \bigtriangledown f =
\bigg(\frac {\partial f}{\partial x},\frac {\partial f}{\partial y},\frac {\partial f}{\partial z}\bigg) \\$$

*$\bigtriangledown f \neq 0 \Rightarrow \bigtriangledown f$ gives direction of f is increasing fastest.

*$\bigtriangledown f$ is normal to Level Surfaces.


##### Tangent Line
![](assets/tangent-line-and-gradient-of-f.png =x250)

$$ l(t) = c(t0) + (t − t0).c'(t0) $$


##### Tangent Planes to Level Surfaces
![](assets/tangent-plane.png =x300)

$$ \text{Tangent Plane} = \bigtriangledown f(x_0,y_0,z_0).(x-x_0, y-y_0, z-z_0) = 0 \\$$

$$ \text{Slope of tangent Plane} = ||\bigtriangledown f|| $$

#### Taylor Theorem

The main point of the single-variable Taylor theorem is to find approximations of a
function near a given point that are accurate to a higher order than the linear approximation.

$$ f(a) + f'(a)(x-a) + \dfrac{f''(a)}{2!}(x-a)^2 + \cdots + \dfrac{f^{(n)}(a)}{n!}(x-a)^n + R_n $$


##### Forms of the Remainder

$$ R_n(x) = \frac {f^{n+1}(c)}{(n+1)!}(x-a)^{n+1} $$

$\exists c$ between $a$ and $x$ such that

##### Arc Length

$$ L = \int_a^b |\overrightarrow {v}|dt =
\int_a^b \sqrt{\Big(\frac {dx}{dt}\Big)^2 + \bigg(\frac {dy}{dt}\bigg)^2 + \bigg(\frac {dz}{dt}\bigg)^2} \\
\text{Arc Length} \\ $$

$$ s(t) = \int_a^b |v(u)|du \\
\text{Arc Length Parameter} \\ $$

$$ s'(t) = |v(t)| \\
\text{Speed on Smooth Curve} \\ $$

##### Tangent Vector
Tangent Vector $\to \overrightarrow{v} = r'(t)$

$$ \overrightarrow{T}(t) = \frac {v}{|v|} = \frac {r'(t)}{|r'(t)|}\\
\text{Unit Tangent Vector} \\ $$

$$ K = \Bigg|\frac {dT}{ds}\Bigg| = \frac {1}{|v|} . \Bigg|\frac {dT}{dt}\Bigg|
= \frac{|v \times a|}{|v|^3} \\
\text{Curvature} \\$$

$$ P = \frac{1}{K} \\ \text{Radius of Curvature} \\ $$

$$ N(t) = \frac{1}{K}.\frac{dT}{ds} = \frac {T'(t)}{|T'(t)|} \\$$

$$ B = T \times N \\ \text{Unit Binormal Vector} \\$$


## Linear Algebra
#### Special Matrices
**1) Square matrix** $A_{nxn}$ (m=n) matrices.

**2) Zero Matrix** $A = A_{ij}$ is a zero matrix if $a_{ij} = 0$  $\forall i,j$.

**3) Diagonal Matrix** If $A$ is square matrix and $a_{ij} = 0$ for $\forall i
\neq j$ and $a_{ij} \neq 0$ for $\exists i = j \Rightarrow$ A is diagonal matrix.

**4) Identity Matrix** $I_{nxn} = (\sigma_{ij})$ and $\sigma_{ij} = \begin{cases}
1, i = j \\
0, i \neq j\\
\end{cases}$

**5) Transpose of a Matrix** $A^t$ is a transpose of $A_{mxn} = (a_{ij})$ if
$A^t_{nxm} = (a_{ji})$

**6) Symmetric Matrix** $A = (a_{ij})$ and $a_{ij} = a_{ji} \Rightarrow$ A is a
symmetric matrix and $A = A^t$

**7) Upper Triangular Matrix** $A = (a_{ij})$ and $a_{ij} = 0$ for $\forall j<i$

**8) Lower Triangular Matrix** $A = (a_{ij})$ and $a_{ij} = 0$ for $\forall j>i$


#### Operations on Matrices
Let $A = (a_{ij}), B = (b_{ij}) ...$

**1) Matrix Addition** For addition, two matrices should have same size. $C = A + B$
and $c_{ij} = a_{ij} + b_{ij}$

**2) Scalar Multiplication** $kA = k(a_{ij})$ for $\forall i,j$

**3) Matrix Multiplication** Let A is an **(mxn)** matrix and B is an **(nxp)**
matrix and let $C = A.B$ where C is **(mxp)** matrix. Then $c_{ij} =
\sum_{k=1}^n a_{ik}b_{kj}$.

Note: Since matrix multiplication need appropriate sizes, when AB exist, BA may not be exist
and if BA exist, $AB \neq BA$ AB and BA can be not equal.

#### Special Products
###### Dot Products
Let $A = (a_{ij}), B = (b_{ij})$ and they **must have same (mxn) size**.
$C = A \cdot B = a_{ij}b_{ij}$

#### Matrix Properties
Let A,B,C are appropriate sized matrices and k is a scalar.

1) $(AB)C = A(BC)$  (associativity)

2) $A(B+C) = AB+AC$ (distributivity)

3) $(A+B)^t = A^t + B^t$

4) $(KA)^t = KA^t$

5) $(A^t)^t = A$

6) $(AC)^t = C^t A^t$


#### Elementary Row Operations

Let rows of matrices defined by $R_1, R_2, ... R_m$. There are 3 **elementary row operation**

M1) Interlope position of two rows (ex. denoted by $R_2 \leftrightarrow R_5$)

M2) Multiply a row by a nonzero constant (ex. denoted by $kR_1$)

M3) Add a multiple of one row to another row (ex. adding $3xR_2$ to $R_3$,denoted by  $3R_2 \rightarrow R_3$)

##### Elementary Row Operation Notes:
**Proposition 1** Any matrix is obtained from A by finite sequence of ERO's (elementary row operations)
is row equivalent to A.


#### Row Echelon Form
**Definition 1** An (mxn) matrix A is said to be in row-echelon form if the following properties all hold;
1) If any rows existing entirely of zeros, they should be at the bottom of rows.

2) The first nonzero element in every nonzero row should be equal to 1 (called leading 1).

3) The leading 1 of any row below the first row is to the right of the leading 1 of the row above it.

**Proposition 1** Any matrix is row equivalent to a row-echelon matrix.

**Proposition 2** Row-echelon form of a given matrix is not unique.

**Proposition 3** All row echelon matrices that are row equivalent to A have the
**same number of nonzero rows**.


#### Reduced Row-Echelon Form
**Definition** An (mxn) matrix is said to be in a reduced row-echelon form if following holds;

1) The matrix should be row-echelon form.

2) Any column that contains a leading 1 has zero everywhere else.

**Note** Identity matrix I is in the reduced row-echelon form

**Proposition 1** The reduced row echelon form is unique.


#### Rank
Rank of matrix is equal to nonzero rows of echelon form of a matrix.

$\ast$ So this means that linear independent 'row' vector count of a matrix.




#### System and Matrix Relation

$$ \text{System} \to \begin{cases}
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b_1\\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_n\\
\end{cases} $$

$$ \text{Matrix form } AX = b \to \begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
\vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}\
\end{bmatrix}

\begin{bmatrix}
x_1 \\
\vdots \\
x_n \\
\end{bmatrix}

=

\begin{bmatrix}
b_1 \\
\vdots \\
b_n
\end{bmatrix}
$$

$$  \text{Augmented Matrix form } [A|b] \to
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} & | & b_1 \\
\vdots & \quad & \quad & \quad & | &  \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} & | & b_n\\
\end{bmatrix}
$$

##### Homogeneity of systems

1) Homogeneous System If all $b_i = 0$  $(AX = 0)$

2) Non-Homogeneous System If $\exists b_i \neq 0$

##### Consistency of systems

1) Consistent System If system has at least one solution.

2) Inconsistent System If system has no solution.


**Note** A system can have **3 type solution**;
1) Unique solution $\rightarrow Rank(A) = Rank[A|b] = n \Rightarrow$ unique solution
2) Infinitely many solution $\rightarrow Rank(A) = Rank[A|b] < n \Rightarrow$ infinitely many solution
3) No solution $\rightarrow Rank(A) \neq Rank[A|b] \Rightarrow$ no solution

#### Equivalent Systems
**Definition** Two linear systems are called equivalent systems if they have exactly
the same solution set.

**Note** Equivalent systems obtained by ERO's. ERO's doesn't change solution sets.

#### Pivot and Free Variables

If a system has augmented matrix in row-echelon form:

a) **Leading 1** variables are called **pivot variables**.

b) Variables which aren't leading 1's and non-zero called free variables.

##### Determinant

$$ det(A)=\displaystyle\sum_{k=1}^{n} a_{ik}C_{ik} $$

$$ \text{where } C_{ij}= (-1)^{i+j}M_{ij} \text{ and } M_{ij} \text{ is the minor of A} $$

$\ast det(A) = det(A^t)$

$det(A) \neq 0 \Rightarrow$ A is invertible and $Rank(A) = n$


### Algebraic Structures

##### Group

- is a set G

- one binary operation defined with properties:

  - Closure: a $\diamond$ b $\in$ G

  - Identity Element: $a \diamond e = e \diamond a = a$

  - Associavity: $a \diamond (b \diamond c) = (a \diamond b)\diamond c$

- is Abelain Group  $\Rightarrow a \diamond b = b \diamond a$


##### Field

- is a set F

- two operation (+), ($\times$) defined:

  - F-{0} is also Abelian Group under ($\times$) operation

##### Vector Spaces

- non-empty set

- two operations defined;

  - addition (+)

  - scalar multiplication ($\times$)

- following properties holds;

  - Closed under $+$ and $\times$

  - Commutative under ($+$)

  - Associative under $+$ and $\times$ ($u+v = v+u$)

  - There exists Additive Identity: $\exists \overrightarrow{0} \in V (u+(-u) =
  (-u)+u=\overrightarrow{0})$

    and Multiplicative Identity ($\overrightarrow{u} \times e = e \times
    \overrightarrow{u} = \overrightarrow{u}$)$

  - Distrubutive $(k \times (\overrightarrow{u} + \overrightarrow{v}) = k
  \overrightarrow{u} + k \overrightarrow{l})$ and $((k+l) \overrightarrow{u} =
  k \overrightarrow{u} + l \overrightarrow{u})$

$\ast$ To determine whether a set V with addition and scalar multiplication
defined on V is a vector space requires verification of the 10 vector space
axioms.

$\ast$ In all vector spaces, additive inverses are unique.

#### Subspace

A subspace W of a vector space V is a nonempty subset that is itself
a vector space with respect to the inherited operations of vector addition and scalar
multiplication on V .



$\ast$ The intersection of any collection of subspaces of a vector space is a subspace of
the vector space.

###### Proving Subspace

$\ast$ If W is nonempty subset of the vector space V, then W is a subspace of V
$\iff$ W is **closed under addition and scalar multiplication** (and $\overrightarrow{0}$ is in W).

To prove that, we need to show $\overrightarrow{u} + (c \cdot \overrightarrow{v})
\in W$ with 3 steps.

Step 1 - Closed Under Addition: Suppose that $\overrightarrow{u}, \overrightarrow{v}
\in W$; then $u + (1 \cdot v) = u + v \in W$

Step 2 - W is Nonempty (has $\overrightarrow{0}$ vector): $\overrightarrow{0} =
u + ((−1) \cdot u)$

Step 3 - Closed Under Scalar Multiplication: $c \times u = 0 + (c \cdot u) \in W$

Step 4 - Converse: if W is a subspace with u and v in W, and c a scalar, then since W
is closed under addition and scalar multiplication, we know that $u + (c \cdot v) \in W$  $\Box$.



##### Polynomial Vector Spaces

$P_n$ the set of all polynomials of degree n or less.

$p(x) = a_0 + a_1 x + a_2 x^2 + · · · + a_{n−1}x^{n−1} + a_n x^n$

$\ast$Note that $V = P_n \cup$ {$0$} is a real vector space, where 0 is the zero polynomial.

$\ast$Note that n degree Polynomial Vector Space's dimension is $dim(P_n) = n+1$



###### Vector Space Properties

-  $\overrightarrow{0}$ vector is unique

- $0 \cdot \overrightarrow{v} = \overrightarrow{0}$ and $k \cdot \overrightarrow{0}
= \overrightarrow{0}$

- Additive inverse of a vector $\overrightarrow{v}$ is unique

- If $k \cdot \overrightarrow{v} = \overrightarrow{0} \Rightarrow k = 0 \vee
\overrightarrow{v} = \overrightarrow{0}$



#### Linear Combination

Linear combination of vectors defined as the form:

$$ (c_1 \cdot \overrightarrow{v_1}) + (c_2 \cdot \overrightarrow{v_2}) + \dots
+ (c_k \cdot \overrightarrow{v_k})$$

$\ast$ Let $u$ and $v$ are vectors in same vector space.  For any scalar $c$,
$u = cv \Rightarrow$ then u is linear combination of v.


#### Linear Dependence

$S = \{v_1, v_2, \dots , v_m \}$ in a vector space V is **linearly independent**
$\Rightarrow c_1 v_1 + \dots + c_m v_m = 0$ is **only have trivial solution**
$c_1 = c_2 = \dots = c_m = 0$.

If the equation has a nontrivial solution the set $S$ is **linearly dependent**.

$\ast$ Linear dependance is a property of vector sets.

$\ast A_{n \times n}$ and column vectors of A  **linearly independent** $\iff det(A) \neq 0$

$\ast A_{n \times n}$ and column vectors of A **linearly independent** $\iff$ A is invertible.

$\ast$ If $\overrightarrow{0}$ vector contained by S, then S is **linearly dependent**.

$\ast$ Let $S = \{v_1, v_2, \dots, v_n\}$ is set of nonzero vectors that in
$R^m$. $n > m \Rightarrow$ S is **linearly dependent**.

$\ast$ Set of nonzero vectors is **linearly dependent** $\iff$ at least one of the vectors
is linear combination of other vectors in the set.

$\ast$ S is **linearly independent** set of vectors $\Rightarrow$ subset of S is
linearly independent.

$\ast$ T is **linearly dependent** set of vectors and S contains T $\Rightarrow$ S is
linearly dependent.

$\ast$ Let $Ax = b$ consistent. The solution is unique $\iff$ column vectors of A
is **linearly independent**.

$\ast$ Let $Ax = 0$. The only solution is trivial $\iff$ column vectors of A
is **linearly independent**.

**Determining set of vectors linearly independent**

Let column vectors

$$ v_1 = \begin{bmatrix}
a_{11} \\
a_{21} \\
\vdots \\
a_{m1} \\
\end{bmatrix}
v_2 = \begin{bmatrix}
a_{12} \\
a_{22} \\
\vdots \\
a_{m2} \\
\end{bmatrix}
\dots
v_n = \begin{bmatrix}
a_{1n} \\
a_{2n} \\
\vdots \\
a_{mn} \\
\end{bmatrix} $$
1) Write column vectors as a linear combination $\to c_1 v_1 + c_2 v_2 + \dots + c_n v_n = 0$

2) obtain a system based on scalars $\to \begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} \\
\end{bmatrix}
=
\begin{bmatrix}
0 \\
0\\
\vdots \\
0 \\
\end{bmatrix}$

3) Solve the system.

4) If only solution is the trivial solution $c_1 = c_2 = \dots = c_n = 0 \Rightarrow$
 vectors are linearly independent.



##### Span of Set of Vectors
Let $S = \{v_1, v_2, \dots ,v_k \}$ be a vector set.

$$ span(S) = \{(c_1 \cdot \overrightarrow{v_1}) + (c_2 \cdot \overrightarrow{v_2})
+ \dots + (c_k \cdot \overrightarrow{v_k})\} $$

##### Proposition - $span(S)$ is a Subspace

$\ast$ If S is a set of vectors in vector space V $\Rightarrow span(S)$ is a **subspace**.

- **Proof**

  $\overrightarrow{u}+c\overrightarrow{w} = (c_1 v_1+ \dots + c_n v_n) +
  c(d_1 v_1 + \dots + d_n v_n) = (c_1 + c d_1)v_1 + \dots + (c_n + c d_n)v_n$

  Since $c_n + c d_n$ is a scalar, $u+cw \in span(S)$, and hence span is a subspace $\Box$.


##### Null Space
Null space of A is the set $N(A) = \{ \overrightarrow{x}: A\overrightarrow{x}
= \overrightarrow{0} , x \in R^n \}$.

##### Column Space

Column space of A is denoted by $col(A)$ is the set of all linear combinations
of column vectors of A.

##### Theorem - $Ax = b$ consistence

Let A be an m × n matrix. The linear system $Ax = b$ is consistent $\iff b
\in col(A)$.


##### Theorem - $N(A)$ and $col(A)$ are Subspace

If $A$ is $m \times n$ matrix, $col(A)$ is subspace of $R^m$ and $N(A)$ is
subspace of $R^n$.


### Basis and Dimension

#### Span
Let $S = \{v_1, v_2, \dots , v_m \}$ and $\forall v \in V$ can be written as
$v = c_1v_1 + c_2v_2 + \dots + c_mv_m \Rightarrow span(S) = V$ (S span V).

Let $dim(V) = n$.

$\ast$ If $k < n \Rightarrow$ $span(S) \neq V$.

**How to show S spans $R^n$**

1) Take $v = (a_1, a_2, \dots, a_n) \in R^n$

2) Let $v = (a_1, a_2, \dots, a_n) = c_1v_1 + \dots + c_n v_n$ s.t. $c_i$ are constants.

3) Show that $\begin{bmatrix}
v_1 & v_2 & \dots & v_k & | & a_1 \\
 \downarrow & \downarrow & \dots & \downarrow & | & \vdots \\
 \quad & \quad & \quad & \quad & | & a_n \\
\end{bmatrix}$ is consistent (by echelon form).

#### Basis for a Vector Space - Definition

If following properties hold:

1) $B$ is linearly independent set ($c_1 v_1 + \dots + c_m v_m = 0$ is **only
have trivial solution**).

2) $B$ spans $V$ (Every item in V should be written as linear combination of
vectors in B).

$B$ is a **basis** for vector space $V$.

$\ast \forall v \in V$ has a unique representation.

**Corollary**
Let $S= \{ v_1, v_2, \dots, v_k \}$ st. $v_1, v_2, \dots, v_k \in V$ and $A =
[v_1|v_2|\dots|v_k]$.
For Rank(V) = n.

- if $k>n$, then S is **linearly dependent**

- if $k=n$ and $det(A) = 0$ (also means that $Rank(A) \neq n$) then S is **linearly dependent**

- if $k=n and $det(A) \neq 0$ (also means that $Rank(A) = n$) then S is **linearly independent**

#### Wronskian of Function set

Function set $S = {f_1, f_2, \dots, f_k}$ where $f_1, f_2, \dots, f_k \in C^{k-1}(I)$
(means that those functions differentiable k-1 times)

$$ W[f_1, f_2, \dots, f_k] = \begin{vmatrix}
f_1(x) & f_2(x) & \dots & f_k(x) \\
\vdots \\
f^{(k-1)}_1(x) & f^{(k-1)}_2 & \dots & f^{(k-1)}_k(x)
\end{vmatrix} $$

$\ast$ Wronskian is scalar since it is a determinant.

$\ast$ If $W[f_1, f_2, \dots, f_k] \neq 0$ for any $x_0 \in I$, then S is linearly independent.

#### Dimension
The number of vectors in any basis for $V$ and denoted by $dim(V)$.

$\ast$ Every basis of V has $n$ vectors.

$\ast$ If $V = \{ \overrightarrow{0} \} \Rightarrow dim(V) = 0$.

$\ast$ $dim(M_{m \times n}(IR)) = m \cdot n$ , $dim(P_n(R))= n + 1$

$\ast$ Let $dim(V) = n$ and $B = \{ v_1, v_2, \dots, v_k \}$ s.t. $v_1, v_2, \dots, v_k \in V$

1) If B linearly independent $\Rightarrow$ B is basis for V (B spans V also).

2) If B spans V $\Rightarrow$ B is basis for V (B is linearly independent also).


#### Ordered Basis

Ordered basis are basis that ordered set of vectors.

#### Transition Matrix of Ordered Basis from B to B'

Let $B = \{ v_1, v_2, \dots, v_n \}$ and $B' = \{ v'_1, v'_2, \dots, v'_n \}$

Transition matrix

$$ [I]^{B'}_B =
\begin{bmatrix}
\left[
v_1
\right]_{B'}
& \left[
v_2
\right]_{B'}
&
\dots
&
\left[
v_n
\right]_{B'}
\end{bmatrix} $$


**Finding Transition Matrix**

1) Let $c_1, c_2, \dots, c_n$ are coordinate vectors. Than solve equation for
$c_1 v'_1 = v_1, c_2 v'_2 = v_2, \dots, c_n v'_n = v_n$

2) Then put them in form of $[I]^{B'}_B = \begin{bmatrix}
c_1 & c_2 & \dots & c_n \\
\downarrow & \downarrow & \dots & \downarrow
\end{bmatrix}$


#### Eigenvalues and Eigenvectors
$A$ is matrix, $\overrightarrow{v}$ is eigenvector and $\lambda$ is eigenvalue.
$$ A \overrightarrow{v} = \lambda \overrightarrow{v} $$

$\lambda$ is eigenvalue of matrix $A \iff det(A-\lambda I) = 0$

$\ast A \overrightarrow{v} = \lambda \overrightarrow{v}$ says that eigenvectors
keep same direction when multiplied by $A$.

$\ast$ The eigenvalues of $A^2 \to \lambda^2$ and $A^{-1} \to \lambda^{-1}$ with the same eigenvectors.

$\ast$ The sum of $\lambda$'s = sum of main diagonal of A.

$\ast$ The product of $\lambda$'s is equal to determinant of A.


**Finding Eigenvalues and Eigenvectors**

1) Compute $det(A - \lambda I) = 0$

2) Find the roots of this polynomial ($\lambda$'s)

3) Solve ($a - \lambda I)\overrightarrow{v} = 0$ to find eigenvectors $\overrightarrow{v}$
