# Linear Algebra Notes

## Linear Transformations

### Linearity Properties for Linear Transformations

1) $T(u+v) = Tu + Tv$
2) $T(cu) = cTu$

Briefly show: $T(cu + v) = cTu + Tv$

### Kernel and Range

$$ Ker(T) = Nullsp(T) = {v \in V: Tv = 0} $$

$$ Range(T) = R(T) = \{w \in W: w = Tv, v \in V\} $$

**Note:** Every vector in $Ker(T)$ is mapped to the zero vector in W.

$$ dim(Ker(T)) + dim(Range(T)) = dimV $$

$$ Nullity(T) + Rank(T) = dimV $$

So, $dim(Ker(T)) = Nullity(T), dim(Range(T)) = Rank(T)$.

### Existance and Uniqueness of Linear Transformation

If $V$ and $W$ are finite dimensional vector spaces over same field, there is **unique** linear tranformation that

Let B is a bases with vectors **$v_i$, $i=\overline{1,n}$**

$$ Tv_i = w_i $$

The set of all linear transformations from V to W is a vector space, denoted by **$L(V,W)$**

### Product (Composition) of Linear Transformations

$T_1 \in L(U,V), T_2 \in L(V.W)$, then

$$ (T_2 T_1)u = T_2(T_1 u) $$

Properties:

1- Associativity:

$$(T_3 T_2)T_1 = T_3 (T_2 T_1)$$

2- Distributivity:

$$ (S_1 + S_2)T = S_1 T + S_2 T $$

$$ S(T_1 + T_2) = ST_1 + ST_2 $$

3- Identity Transformation:

$$ I_v: V \rightarrow V $$

$$ I_w: W \rightarrow W $$

Then,

$$ TI_v = T, TI_w = T $$

### One-to-one and onto

$T$ is **one-to-one** $\iff$ $T$ maps **every linearly independent set of vectors** in V to W.

$T$ is **one-to-one** $\iff Ker(T) = {0}$

$T$ is **onto** $\iff Range(T) = W$ .

1) If $T$ is **one-to-one** $\Rightarrow dimV \leq dimW$

2) If $T$ is **onto** $\Rightarrow dimV \geq dimW$

3) If $T$ is **one-to-one and onto (bijective)** $\Rightarrow dimV = dimW$

### Invertibility

$T$ is invertible if $\exists S: W \rightarrow V$ s.t.

$$ ST = I_v \quad \mathrm{and} \quad TS = I_w$$

$S$ is called inverse of T.

$T$ is **invertibe** $\iff$ $T$ is **one-to-one and onto**.

If $dimV = dimW = n$, then followings are equal:

1) $T$ is **invertible**

2) $T$ is **one-to-one**

3) $T$ is **onto**

### Coordinate Representation of Vectors

Let $\beta = \{v_1, \dots,v_n\}$ is a ordered bases of $V$. Then $\forall v \in V$ has a unique representation:

$$ v = c_1v_1 + \dots + c_nv_n $$

coordinate vector of v related to the base $\beta$ is

$$ [v]_\beta = [c_1 \dots c_n]^t = \begin{bmatrix} c_1 \\ \vdots \\ c_n \end{bmatrix} $$

Transformation $L_0: V \to M_{nx1}$ is: $L_0(v) = [v]_\beta$

1) is one-to-one and onto (invertible)

2) is linear

Thus, $L_0$ is an isomorphism.

#### Transition matrix $P$

Let $dimV=n$, $\beta = \{v_1, \dots, v_n\}$ and $\Upsilon = \{u_1. \dots, u_n\}$ be two **ordered** bases.

Then, there exists a unique invertible (nxn) matrix $P$ s.t.

**$$ [v]_\beta P[v]_\Upsilon, \forall v \in V $$**

and since $P$ is invertible.

**$$ [v]_\Upsilon = P^{-1}[v]_\beta $$**

where

$$ P = \begin{bmatrix} [u_1]_\beta & \dots & [u_n]_\beta \\ \downarrow & \downarrow & \downarrow \end{bmatrix} = [p_{ij}] $$

and $P$ is called **transition matrix**.

#### Matrix Representation of Operator T

**Every linear transformation defined on a finite dimensional space can be represented by a matrix.**

Matrix $A$ is called the matrix representation of operator $T$ relative to the bases $\beta , \Upsilon$ for $V$ and $\beta^\prime , \Upsilon^\prime$  for $W$. Then, for each linear transformation $T: V \to W$ there is a **unique** matrix $A_{mxn}$.

$A = [T]_{\beta}^{\beta^\prime} = \begin{bmatrix} [Tu_1]_{\beta^\prime} & \dots & [Tu_n]_{\beta^\prime} \\ \downarrow & \downarrow & \downarrow \end{bmatrix} $

and satisfying

$$ A[v]_\beta = [Tv]_{\beta^\prime} \quad , \forall v \in V $$

This means that, for given $\beta$ and $\beta^\prime$, the correspondance $T \overset{L_0}{\longmapsto}[T]_\beta^{\beta^\prime}$ defines a mapping $L_0: L(V,W) \to M_{mxn}$

1) This mapping is **linear**

2) This mapping is **one-to-one and onto (invertible)**

Notations for 2 case:

1) If $\beta \neq \beta^\prime \implies A = [T]_\beta^{\beta^\prime}$ then,

$$ [T]_\beta^{\beta^\prime} [v]_\beta = [Tv]_{\beta^\prime} \quad , \forall v \in V $$

2) If $\beta = \beta^\prime \implies A = [T]_\beta$, then

$$ [T]_\beta[v]_\beta = [Tv]_\beta $$

With two different bases, let P be be the transition matrix from $\beta \to \Upsilon$ and Q from $\beta^\prime \to \Upsilon^\prime$.

$$ [T]_\Upsilon^{\Upsilon^\prime} = Q^{-1} [T]_\beta^{\beta^\prime}P $$

---

If $T:V \to V$ is a linear operator and $\beta, \Upsilon$ two bases for $V$, and $P$ is transition matrix s.t.

$$ [v]_\beta = P[v]_\Upsilon$$

then relation between representations $[T]_\beta$ and $[T]_\Upsilon$ is:

$$ [T]_\Upsilon = P^{-1}[T]_\beta P $$

---

Two vector spaces $V$ and $W$ over the same field that is **isomorphic** notated as $V \overset{\sim}{=} W$.

---

#### Isomorphism Properties

Isomorphism is an equivalence relation on the set of all n-dimensional vector spaces over the same field. That's, if $U,V,W$ are any n-dimensional vector spaces over $\mathbb{F}$, then

1) $V \overset{\sim}{=} V$ (reflexive)

2) $V \overset{\sim}{=} U \implies U \overset{\sim}{=}V$ (symmetric)

3) $V \overset{\sim}{=} U and U \overset{\sim}{=}W \implies V \overset{\sim}{=} W$ (transitive)

Then,

$$ V_\mathbb{F} \overset{\sim}{=} M_{nx1}(\mathbb{F}) \overset{\sim}{=} \mathbb{F}^n $$

$$v \longleftrightarrow \begin{bmatrix} x_1 \\ \vdots \\ x_n  \end{bmatrix} \longleftrightarrow (x_1, \dots, x_n)$$

---

Let $dimV = n$ and $dimW = m$

Then,

$$ L(V,W) \overset{\sim}{=} M_{mxn}(\mathbb{F})$$

and

$$ dimL(V,W) = dimM_{mxn} = m \cdot n $$

---

### Sum and Direct Sum

Let $U_1, \dots, U_m$ be subspaces of V. Then the **sum of $U_1, \dots, U_m$** is defined as

$$ U_1 + \dots + U_m = \{ u_1 + \dots + u_m : u_j \in U_j, j= \overline{1,m} \}$$

if each element $v \in V$ **has a unique** representation as a sum $\implies$ V is the **direct sum** its subspaces $U_!, \dots, U_m$ written as

$$ V = U_1 \oplus \dots \oplus U_m$$

$$ v = u_1 + \dots + u)m$$

where $u_j \in U_j, j = \overline{1,m}$

---

If V is a finite dimensional vector space and $U$ is subspace of V, $\exists W$ subspace of V s.t.

$$ V = U \oplus W $$

---

$$ V = U_1 \oplus \dots \oplus U_m$$

$$ \iff $$

1) $v = U_1 + \dots + U_m$

2) $u_1 + \dots + u_m = 0 \implies u_j = 0 \quad , \forall j = \overline{1,m}$

---

Let $U,W$ be subspaces of V, then

$$ V = U \oplus W $$

$$ \iff $$

$$ V = U + W \quad \mathrm{and} \quad U \cap W = \{0\} $$

---

A mapping $T: V \to V$ that is linear, called **linear operator**. In that case $T \in L(V)$.

For $U_j$ that is subspace of V, restriction of T to smaller domain $U_j$ notated as $T|_{U_j}$

The subspace $U$ is called to be **invariant under operator T** if $u \in U \implies Tu \in U$.

(In other words, $U$ is **invariant under $T$** if $T|_U$ is an operator on $U$.

---

#### Linear Operator Properties

1) $\{0\}$ is **invariant** under $T$.

2) $V$ is **invariant** under $T$.

3) $Ker(T)$ is **invariant** under $T$.

4) $Range(T)$ is **invariant** under $T$.

---

#### Projection Operators in Vector Space

Let $V = U \oplus W$, then $P: V \to V$ is called **projection operator** that maps V onto W along U, if $\forall v \in V$ having a **unique** representation

$$ v = u + w$$

we define

$$ Pv = w$$

**Moreover**, ($I-P$) is a projection of V onto U, where $I$ identity operator on $V$.

Also, $U = Ker(P), \quad W=Range(P)$.

##### Properties

1) $P$ is a **linear operator**.

2) $P^2 = P$ ($P$ is ideupatent operator).

3) $Pw = w \iff w \in Range(P)$.

---

### Eigenvalue and Eigenvector of Linear Transformations

Let $T \in L(V)$ is a **linear operator**.

1) An **eigenvalue** of $T$ is a scalar $\lambda$ s.t. $\exists v \in V \quad v \neq 0$ satisfying $Tv = \lambda v$. $v$ is **eigenvector**.

2) The subspace $W_\lambda$ that $W_\lambda = \{ \forall v \in V : Tv = \lambda v, \quad \lambda \in \mathbb{F} \}$ is called **eigenspace**.

---

The set of all **eigenvalues** of $T$ is called **spectrum** of $T$, denoted by $spec(T)$.

$$ spec(T) = \{ \lambda \in \mathbb{F} : Tv = \lambda v \quad , \exists v \in V \} $$

* **existance of eigenvalues depends on the field $\mathbb{F}$ whether is real or complex.**

---

**Every linear operator $T: V \to V$** where V is a finite dimensional vector space over the field of **complex numbers has at least one eigenvalue**.

---

$T$ is a linear operator, if $\lambda_1,\dots,\lambda_m$ are **distinct eigenvalues** of T, and $u_1, \dots, u_m$ are corresponding **eigenvectors**, then set of these eigenvectors $\{ u_1, \dots, u_m \}$ is a **linearly independent set**.

---

If $dimV = n \implies T$ **has at most** n distinct eigenvalues.

---

#### Fan of Subspaces of V and Triangular Matrix Representations

The set $\{W_1, \dots, W_n\}$ of subspaces of V is called a **fan of T** in $V$, if the followings hold:

1) $W_1 \subset \dots \subset W_n = V$

2) $dim(W_k) = k$ for $\forall k = \overline{1,n}$

3) $W_k$ is **invariant** under T, that's $T(W_k) \subseteq W_k \quad , \forall k = \overline{1,n}$

---

If $\{W_1, \dots, W_n\}$ is a fan of T, then $\beta = \{ v_1, \dots, v_n \}$ is called a fan basis for $V$, if

$\{ v_1 \}$ is a basis for $W_1$

$\quad \vdots$

$\{ v_1, \dots, v_n \}$ is a basis for $W_n = V$

---

If $T \in L(V)$ and $\beta$ is a fan basis for $V$, then the matrix representation of $T$ w.r.t. $\beta$ is **upper trianguler**.

---

Let $T \in L(V)$ and $\beta = \{ v_1, \dots, v_n \}$ is a basis of V. Then the followings are equivalent.

1) The matrix of T w.r.t. basis $\beta$ is **upper triangular**.

2) $T v_k \in W_k = span\{ v_1, \dots, v_k \}$ for each $k = \overline{1,n}$

3) $W_k = span\{ v_1, \dots, v_k \}$ is **inavriant** under T for each $k = \overline{1,n}$

---

If $T \in L(V)$ and V is a finite dimensional vector space over the field of **complex numbers**, then $\exists$ a fan of T in V.

Every lin. op. T defined on a **complex** vector space V can be represented by a **triangular matrix$$.

### Diagonalizable Matrices

A square matrix $A_{nxn}$ is **diagonalizable** if $\exists P$ that is invertible s.t.

$$ P^{-1}AP = D $$

A lin. op. T defined on a finite dim. v.sp. V is **diagonalizable** if basis $\exists \beta$ for V s.t. the **matrix representation of T w.r.t. this basis is diagonal**, that

$$ [T]_\beta = D $$

**not every operator diagonalizable, even in complex vector space.**

---

$T \in L(V)$ on a finite dim. v.sp. V is diagonalizable $\iff$ there exists a basis $\beta$ for V consisting entirely of **eigenvectors** of T.

---

$T \in L(V)$ on v.sp. V with $dimV = n$. If $T$ has n distinct **eigenvalues**, then $T$ is diagonalizable.

---

$T \in L(V)$ and $dimV = n$. Let $\lambda_1, \dots, \lambda_m$ be the **distinct eigenvalues of $T$** and $W_i = Ket(T - \lambda T) \quad, i=\overline{1,m}$ denote the correspondant eigenspaces. Then, the followings are equivalent

1) $T$ is **diagonalizable** operator.

2) $V$ has a **basis consisting of eigenvectors** of op. $T$.

3) There exists one-dimensional subspaces $U_1, \dots, U_n$ of V, each of which is **invariant** under T, and $V = U_1 \oplus \dots \oplus U_n$.

4) $V = W_1 \oplus \dots W_m \quad , W_i = Ker(T-\lambda_i I)$.

5) $dimV = dimW_1 + \dots + dimW_m$

---

#### Remember for Matrices

* If $A_{mxn}$ and $m \neq n$, then we **can not define powers** of $A$.

* If $A_{nxn}$ is a square matrix, then we **can define the powers of $A$** $A,A^2, \dots, A^k, \quad k = 1,2,\dots$

---

##### Similarly

* If $T: V \to W$ is a linear mapping and $V \neq W$, then we **can't define the powers of T**.But,

* if $T \in L(V)$ then powers of T are defined as:

$T^2 = TT$

$T^3 = TTT$

$\quad \vdots$

$T^m = \underbrace{T \dots T}_{\mathrm{m \hspace{2px} times}}$

and $T^0 = T$

---

### Invariant Subspaces on Real Vector Spaces

* On a **Complex Vector Space V** **every linear operator T** has an **eigenvalue** and therefore has an **eigenvector**. It means, in complex spaces a linear opreator always has an **invarian** subspace of dimension 1.

* On a **Real Vector Space V** a linear operator **may not have** an **eigenvalue**, and therefore **may not have an invariant subspace** of dimension 1. However, an invariont subspace of dimension  1 or 2 **always exist**.

**Remember**, T has a 1-dimensional invariant subspace $\iff$ T has an eigenvalue(eigenvector).

---

**Every** lin. op. T on a finite-dimensional, nonzero, **real vector space V** has an **invariant subspace of dimension 1 or 2**.

---

Every operator T on a **odd-dimensional real v.sp. V** has an eigenvalue.

---

### Inner Product Spaces

---

#### Introduction

1) Vector Space operations $\to \begin{cases} u + v \quad \mathrm{(addition)} \\ \alpha u \quad \mathrm{(scalar} \hspace{2px} \mathrm{multiplication)}  \end{cases}$

2) Inner Product Space $\to$ Vector Space $+$ inner product $<u,v>$

* In every inner product space one has Norm: $||u|| = \sqrt{<u,v>}$, Distance: $||u-v|| = \sqrt{<u-v,u-v>}$

* Most important notion in inner product spaces: **Orthogonality**: $<u,v> = 0$

---

* An **inner product** on a vector space is a **function** that takes **each ordered pair $(u,v) \in X \times X$** to a number $<u,v> \in \mathbb{F}$ and satisfies the following properties $\forall u,v,w \in X, \quad \alpha \in \mathbb{F}$:

1) $<u,v> \geq 0$ for $\forall v \in X$ **(positivity)**

2) $<v,v> = 0 \iff v = 0$ **(definiteness)**

3) $<u + v, w> = <u,w> + <v,w>$ **(additivity in first component)**

4) $<\alpha u, v> = \alpha <u,v>$ **(homogenity in first component)**

5) $<u,v> = \overline{<v,u>}$ **(conjugate symmetry)**

* **Inner product space $X$ is a vector space** on which an **inner product (function) defined**: $\{ X, <.,.> \}$

* If $\mathbb{F} = \mathbb{R}$ then complex conjugation is not needed, else $(\mathbb{F} = \mathbb{C})$ complex conjugation needed.

---

If $X$ is an inner product space with an inner product $<u,v>$ defined on it, then $\forall u,v,w \in X$ and $\forall \alpha \in \mathbb{F}$

1) $<0,u> = 0$

2) $<u,0> = 0$

3) $<u, v+w> = <u,v> + <u,w>$

4) $<u, \alpha v> = \overline{\alpha} <u,v>$

5) $ <\alpha u, \beta_1 v_1 + \beta_2 v_2> = \alpha \overline{\beta_1} <u,v_1> + \alpha \overline{\beta_2} <u,v_2>$

6) $<u, \sum_{i = 1}^n> = \sum_{i=1}^n \overline{c_i}<u,v_i>$

---

#### Norm of a Vector

Let $X$ be an inner product space. Then, the orml of $v \in X$ is $||v|| = \sqrt{<v,v>}$.

Then,

1) $||v|| \geq 0$ and $||v|| = 0 \iff v = 0$

2) $||\alpha v|| = ||\alpha|| ||v||$

3) $||u + v|| \leq ||u|| + ||v||$ (Triangle Inequality)

Hence every inner product space is also a normed space.

---

#### Orthogonality

Let $X$ be an inner product space. Two vectors $u,v \in X$ are orthogonal if $<u,v> = 0$.

##### Pythogorean Theorem

If $u$ and $v$ orthogonal vectors in $X$ then $||u + v||^2 = ||u||^2 + ||v||^2$

##### Cauchy-Schwartz Inequality

If $u,v \in X$ then $|<u,v>| \leq ||u||.||v||$

##### Parallelogram Equality

If $u,v \in X$ then $||u+v||^2 + ||u-v||^2 = 2(||u||^2 + ||v||^2)$

---

#### Distance

Distance between two vector is: $||u-v|| = \sqrt{<u-v, u-v>}$

### Orthonormal Set Of Vectors

A set of vectors in an inner product space $X$ $S = \{ u_1, \dots, u_m \}$ is said to be orthonormal if

$$<u_i,u_j> = \delta _{ij} = \begin{cases} 1, i=j \\ 0, i \neq j \end{cases}$$

If the set $S$ is **orthonormal**, then it is **linearly independent**.

If the set $S$ is **orthonormal**,

$$||c_1u_1 + \dots + c_mu_m||^2 = |c_1|^2 + \dots + |c_m|^2 = ||\sum_{i=1}^m c_i u_i||^2 = \sum_{i=1}^m |c_i|^2$$

### Orthonormal Basis

Let $X$ be an inner pr. sp. over $\mathbb{F}$. A set of vectors in $X$, say $\beta_0 = \{u_1, \dots, u_n \}$ is an **orthonormal basis** for $X$ if

$$dimX = n \quad \mathrm{and} \quad <u_i,u_j> = \delta_{ij}, \quad \forall i,j = \overline{1,n}$$

---

If $X$ is an inner product space and $\beta_0$ is an orthonormal basis for $X$ then every $v \in X$ has the unique representation

1) $v = \sum_{i=1}^n <v,u_i>u_i$,

2) $||v||^2 = \sum_{i=1}^n |<v,u_i>|^2$

### TODO: Gram-Schmidt Procedure (Page 101)

---

Every finite-dimensional inner product space has an orthonormal basis.

---

Every orthonormal set of vectors in $X$ can be extended to an orthonormal basis for $X$.

### Orthogonal Projection Operator

If $U$ is a subset of an inner product space $X$ then the **orthogonal compliment** of $U$, denoted by $U^\perp$, is the set of all vectors in $X$ that are orthogonal to **every** vector in $U$:

$$ U^\perp = \{ w \in X : <w,u> = 0 \quad \forall u \in U \} $$

---

$U^\perp$ is always a **subspace of $X$**. Take $w_1,w_2 \in U^\perp$, then by defn.

$$ <w_1,u> = 0, <w_2,u> = 0 \quad \forall u \in U$$.

It follows that

$$ <\alpha w_1 + w_2, u> = \alpha <w_1,u> + <w_2,u> = 0 \quad \forall u \in U$$

$$ \implies \alpha w_1 + w_2 \in U^\perp $$

**$\implies U^\perp$ is a subspace**.

* **Note that**, $X^\perp = \{0\}, \quad \{0\}^\perp = X$

---

If $U$ is a subspace of an inner product space $X$ then 

$$ X = U \oplus U^\perp$$

---

Let $X = U \oplus U^\perp$, which means any $v \in X$ has a unique representation.

1) $v = u + w, \quad u \in U, \quad w \in U^\perp$

Then the operator $P : X \to X$ defined as

2) $Pv = u, \quad \forall v \in X$

is called **orthogonal projection** of $X$ onto $U$.

clearly, $\begin{cases}  Ker(P) = U^\perp \\ Range(P) = U \end{cases}$

* Also, $(I-P)v = w \in U^\perp$ is an orthogonal projection of $X$ onto $U^\perp$

* Moreover, one can show that

1) $P^2 = P$

2) $||Pv|| \leq ||v||, \quad \forall v$

---

### TODO: The Best Approximation (Minimizin The Error) (Page 106)

---

### Linear Functions and Adjoint Operators

#### Linear Functionals on Vector Spaces

A **linear mapping** $f$ from v.sp. $V$ to the field $\mathbb{F}$ is called a **linear functional** and we write $f: V \to \mathbb{F}$ or $f \in L(V, \mathbb{F})$.

So, a linear functional $f: V \to \mathbb{F}$ is a special linear transformation, where the **output space** is $\mathbb{F} (\mathbb{R}$ or $\mathbb{C})$

##### Notes

Since linear functionals special linear maps then we can use our previous knowledge to say that:

1) If $f: V \to \mathbb{F}$ is a nonzero linear functional, then $Range(f) = \mathbb{F}$ (one-dimensional)

2) **By dimension theorem**, $dim(Ker(f)) + dim(Range(f)) = dimV$. If $dimV = n \implies dim(Ker(f)) = n -1$, since $dimRange(f) = 1$

3) **By Existance and Uniqueness Theorem** for linear transformations,  a linear function $f: V \to \mathbb{F}$ is uniquely determined by its action on basis vectors $\beta = \{ v_1, \dots, v_n \}$ of $V$.

* The collection of all linear functionals on a v. sp. $V$ over $\mathbb{F}$ forms a vector space denoted by $V^* = L(V,\mathbb{F})$.

---

### Linear Functionals on Inner Product Spaces

Linear functionals on inner product spaces have some special properties, which we will describe now.

**First**, let $X$ be an inner product space over $\mathbb{F}$. Then, for given any $w \in X$, the inner product function

$$ f(v) = <v,w>, \quad \forall u \in V$$

defines a linear functional.

This is because inner product is linear in the first variable $v$ i.e.

$$ f(\alpha v_1 + v_2) = <\alpha v_1+ v_2, w> = \alpha <v_1, w> + <v_2, w> $$\

$$ \alpha f(v_1) + f(v_2) $$

**Conversely**, next theorem shows that every linear functional $f: X \to \mathbb{F}$ can be represented **as an inner product**.

#### Riesz Representation Theorem (RRT) (for finite-dimensional inner product spaces)

Let $X$ be a finite-dimensional inner product space over $\mathbb{F}$.

If $f: X \to \mathbb{F}$ is a linear functional on $X$, then there exists a unique vector $w \in X$ s.t. 

$$ f(v) = <v,w>, \quad \forall v \in X$$

#### The Adjoint Operator

Let $V$ and $W$ be finite dimensional inner product spaces.

If $T: V \to W$ is a linear transformation, there exists a unique linear transformation $T^*: W \to V$ s.t.

$$ <Tv, w>_W = <v, T^*w>_W. \quad \forall v \in V, \quad \forall w \in W$$

---

If $T: V \to W$ is a linear transformation, then $T^*: W \to V$ is called the adjoint of T if

$$ <Tv,w> = <v, T^*w>, \quad \forall v \in V, \quad \forall w \in W$$

##### Properties of Adjoint

If $T,S \in L(V,W), \quad \alpha \in \mathbb{F}$ then

1) $(T + S)^*=T^* + S^*$ **(additivity)**

2) $(\alpha T)^*=\overline{\alpha} T^*$ **(conjugate homogenity)**

3) $(T^*)^* = T$

4) $(ST)^*=T^* S^*$ for $T \in L(V,W)$ and $S \in L(W,U)$

5) $(T^*)^{-1}=(T^{-1})^*$

---

Let $T \in L(V,W)$. Then,

1) $Ker(T^*) = (Range(T))^\perp$

2) $Range(T^*) = (Ker(T))^\perp$

3) $Ker(T) = (Range(T^*))^\perp$

4) $Range(T) = (Ker(T)^*)^\perp$

according to that, these are always true

$$ V = Ker(T) \oplus (Ker(T))^\perp = R(T^*) \oplus (R(T^*))^\perp$$

$$ W = R(T) \oplus (R(T))^\perp = Ker(T^*) \oplus (Ker(T^*))^\perp$$

This proposition says that: $\begin{cases} V = Ker(T) \oplus R(T^*) \\ W = Ker(T^*) \oplus R(T) \end{cases}$

---

### Matrix Representation using Orthonormal Bases

Let $V$ be an inner pr. sp. with orthonormal basis $\beta = \{ v_1, \dots, v_n \}, \quad dimV = n$

and $W$ be an inner pr. sp. with orthonormal basis $\Upsilon = \{ w_1, \dots, w_m \}, \quad dimW = m$

---

If $T: V \to W$ is a linear transformation, then

$$ [T]_\beta^\Upsilon = \begin{bmatrix}
<Tv_1, w_1> & \dots & <Tv_n, w_1> \\
<Tv_1, w_2> & \dots & <Tv_n, w_2> \\
\vdots & \vdots & \vdots \\
<Tv_1, w_m> & \dots & <Tv_n, w_m>
\end{bmatrix}$$

or briefly

$$ [T]_\beta^\Upsilon = A = (<Tv_j, w_i>) = (a_{ij}), \quad j=\overline{1,n}, \quad i=\overline{1,m} $$

---

If $T^* : W \to V$ is the adjoint of $T: V \to W$, then 

$$ [T^*]_\Upsilon^\beta = \begin{bmatrix}
\overline{<Tv_1, w_1>} & \dots & \overline{<Tv_n, w_m>} \\
\overline{<Tv_2, w_1>} & \dots & \overline{<Tv_n, w_m>} \\
\vdots & \vdots & \vdots \\
\overline{<Tv_n, w_1>} & \dots & \overline{<Tv_n, w_m>}
\end{bmatrix}$$

---

If $A = [T]_\beta^\Upsilon$ is the matrix representation of T w.r.t. orthonormal bases $\beta$ and $\Upsilon$, and $B = [T^*]_\Upsilon^\beta$ is the matrix representation of $T^*$, then

$$ B = \overline{A}^t, \quad \mathrm{i.e.} [T^*]_\Upsilon^\beta = (\overline{[T]}_\beta^\Upsilon)^t $$

* **Note**: With respect to nonorthonormal bases, the matrix of $T^*$ does not necessarily equal the conjugate transpose of the matrix of $T$.

---

### Special Operators in Inner Product Spaces and The Sepctral Theorem

$V \to$ finite dimensional inner product space

$T: V \to V$ linear operator

$T^*: V \to V$ adjoint operator of $T$ defined as $<Tu,v> = <u,T^* v>, \quad \forall u,v \in V$

---

In this chapter we will study:

1) Self-Adjoint ops. $(T = T^*)$

2) Normal ops. $(TT^* = T^*T)$

3) Complex Spectral Theorem

4) Real Spectral Theorem

---

Inclussion of some classes of operators:

Orthogonal Adjoint $\subset \overbrace{Self-Adjoint}^{T=T^*} \subset \overbrace{Normal \hspace{2px} Ops.}^{TT^* = T^*T} \supset \overbrace{Unitary \hspace{2px} Ops.}^{TT^* = T^*T = I}$

---

#### Analogy with Complex Numbers : $z \in \mathbb{C}$

1) $z = \overline{z} \implies z$ is real

2) $z = -\overline{z} \implies z$ is pure imaginary

3) $z\overline{z} = |z|^2 = 1 \implies z$ on the unit circle

4) $z\overline{z} = \overline{z}z \implies$ any $z$

#### Self-Adjoint Operators

T is called self-adjoint if

$$T = T^* \quad i.e. \quad <Tu,u> = <u,Tv>, \quad \forall u,v \in V$$

* If $T = T^*$, then its matrix representation with respect to an orthonormal basis $\beta$ for $V$, say $A = [T]_\beta$ is **Hermitian**, that's $A = A^t$, when $\mathbb{F} = \mathbb{C}$.

* If $T = T^*$, then $A = [T]_\beta$ is **symmetric**, that's $A = A^t$, when $\mathbb{F} = \mathbb{R}$.

* Every complex number can be written using two real numbers. Similarly, any operator can be written in terms of two self-adj. ops.

any $z \in \mathbb{C} \implies z = \underbrace{\frac{1}{2}(z+\overline{z})}_\mathrm{real}+i.\underbrace{\frac{1}{2i}(z-\overline{z})}_\mathrm{real}$

any $T$ linaer $\implies T = \underbrace{\frac{1}{2}(T+T^*)}_\mathrm{self-adj} + i.\underbrace{\frac{1}{2}(T-T^*)}_\mathrm{self-adj}$

#### Eigenvalues and Eigenvectors of Self-Adj Ops

1) Every eigenvalue of a self-adj operator is **real**.

2) Eigenvectors of a self-adj op. corresponding to **distinct** eigenvalues are orthogonal.

---

If $V$ is a **complex** inner product space and $T:V \to V$ is any linear operator s.t. $<Tv,v> = 0$ for $\forall v \in V$, then $T = 0$.

* **Note**: This is false for **real** inner product spaces.

---

Let $V$ be a **complex** inner product space and $T \in L(V)$. Then,

$T$ is self-adj $\iff <Tv,v> \in \mathbb{R}$ for $\forall v \in V$

---

If $T$ is **self-adj.** op. on $V$ s.t. $<Tv,v> = 0$ for $\forall v \in V$, then $T = 0$.

---

#### Existance of Eigenvalue(Eigenvector) of a Self-Adjoint Operator

Let $T$ be a self-adjoint operator on $V$. If $\alpha,\beta \in \mathbb{R}$ satisfy $\alpha^2 < \mu\beta$, then $T^2 + \alpha T + \beta I$ is **invertible**.

---

A **self-adj.** op. $T: V \to V$ on a finite dim. Complex or Real inner product space **has an eigenvalue(eigenvector)**.

---

### Normal Operators

We expect natural generalizations of complex numbers ($z\overline{z}=\overline{z}z) only when operators commute. Thus we look at normal operators.

---

A linear op. T is **normal** if $TT^*=T^*T$. ($T$ and $T^*$ commute).

---

A linear op. T is **normal** $\iff ||Tv|| = ||T^*v||, \quad \forall v \in V.$

---

Let T be a normal op. A vector $v \neq 0$ is an eigenvector of $T$ with an eigenvalue $\lambda \iff v$ is an eigenvector of $T^*$ with eigenvalue $\overline{\lambda}$. That's for normal op.

$$Tv = \lambda v \iff T^*v = \overline{\lambda}v$$

---

If T is **normal**, then eigenvectors of $T$ corresponding to **distinct** eigenvalues are **orthogonal**.

---

### The Spectral Theorem

* Our goal was to learn more about the structure of linear operators.

* In applications, one of the most important operators are the diagonalizable ones.

* If $V$ is a **vector space**, $dimV = n$, then we have seen that $T: V \to V$ is diagonalizable $\iff$ it has n-linearly independent eigenvectors.

* If $V$ is an **inner product space**, then **the spectral theorem** gives the necessary and sufficient conditions, under which a linear $T: V \to V$ is unitarily diagonalizable. We shall see that these are precisely the operators $T \in L(V)$, s.t. $V$ has an **orthonormal basis** consisting of eigenvectors of $T$.

* The structure of these operators depend on the field $\mathbb{F}$. Namely, we have

1) Complex Spectral Theorem (Normal Ops.)

2) Real Spectral Theorem (Self-Adj. Ops.)

---

Let $V = \oplus W^\perp$ be a finite dimensional inner product space, and $T: V \to V$ be any linear operator. If $W$ is invariant under $T$, then $W^\perp$ is invariant under $T^*$.

#### Complex Spectral Theorem

Suppose that $V$ is a **complex** inner product space and $T \in L(V)$. Then, $V$ has an orthonormal basis consisting of eigenvectors of $T \iff T is normal$.

---

#### Real Spectral Theorem

Suppose that $V$ is **real** inner product space and $T \in L(V)$. Then,

$V$ has an orthonormal basis consisting of eigenvectors of $T \iff T$ is self-adjoint.