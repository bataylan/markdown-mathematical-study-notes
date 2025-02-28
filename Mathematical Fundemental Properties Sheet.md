#Common Mathematical Subjects

##Trigonometry
![](triangle-trigonometry.jpg =x250)

###Trigonometric Graphs
####Sinus Graph
![](assets/sinus-graph.png =x250)

####Cosinus Graph
![](assets/cosinus-graph.png =x250)

####Tangent Graph
![](assets/tangent-graph.png =x300)

####Cotangent Graph
![](assets/cotangent-graph.png =x300)

####Secant Graph
![](assets/secant-graph.png =x300)

####Cosecant Graph
![](assets/cosecant-graph.png =x300)

####Trigonometric Values
![](assets/trigonometric-values-table.png =x400)

####Identities
$$\cos^2(\theta)+sin^2(\theta) = 1$$
$$ 1+\tan^2(\theta) = \sec^2(\theta) $$
$$ 1+\cot^2(\theta) = \csc^2(\theta) $$

$$ \cot(\theta) = \frac {1}{\tan(\theta)} = \frac {\cos(\theta)}{\sin(\theta)} $$
$$ \csc(\theta) = \frac{1}{\sin(\theta)} $$
$$ \sec(\theta) = \frac{1}{\cos(\theta)} $$

####Addition Formulas
$$ \cos(A \pm B) = \cos(A).\cos(B) \mp \sin(A).\sin(B) $$
$$ \sin(A \pm B) = \sin(A).\cos(B) \pm \cos(A).\sin(B) $$
$$ \tan(A \pm B) = \frac {\tan(A) \pm \tan(B)}{1 \mp \tan(A)\tan(B)} $$

####Double Angle Formulas
$$ \cos(2\theta) = \cos^2(\theta)-\sin^2(\theta) $$
$$ \sin(2\theta) = 2\sin(\theta)\cos(\theta) $$
$$ \tan(2\theta) = \frac {2\tan(\theta)}{1-\tan^2(\theta)} $$
$$ \cot(2\theta) = \frac {\cot^2(\theta) - 1}{2\cot(\theta)} $$

####Half-Angle Formulas
$$ \cos\Big(\frac{\theta}{2}\Big) = \pm \sqrt{\frac{1 + \cos(\theta)}{2}} $$
$$ \sin\Big(\frac{\theta}{2}\Big) = \pm \sqrt{\frac {1 - \cos(\theta)}{2}}  $$
$$ \tan\Big(\frac{\theta}{2}\Big) = \pm \sqrt{\frac {1 - \cos(\theta)}{1 + \cos(\theta)}}
= \frac{\sin(\theta)}{1+\cos(\theta)} = \frac {1-\cos(\theta)}{\sin(\theta)} $$

###Hyperbolic Function
$$ \sinh(x) = \frac {\mathrm{e}^x - \mathrm{e}^{-x}}{2} $$
$$ \cosh(x) = \frac {\mathrm{e}^x + \mathrm{e}^{-x}}{2} $$
$$ \tanh(x) = \frac {\sinh(x)}{\cosh(x)}
= \frac {\mathrm{e}^x - \mathrm{e}^{-x}}{\mathrm{e}^x + \mathrm{e}^{-x}} $$
$$ \coth(x) = \frac {\cosh(x)}{\sinh(x)}
=\frac {\mathrm{e}^x + \mathrm{e}^{-x}} {\mathrm{e}^x - \mathrm{e}^{-x}} $$

$$ \mathrm{sech(x)} \frac {1}{\cosh(x)} $$
$$ \mathrm{cosech(x)} = \frac {1}{\sinh(x)} $$

####The Law Of Cosines
$$ c^2 = a^2 + b^2 - 2ab\cos(\theta)$$

####Eular Formulas
$$ \mathrm{e}^{ix} = \cos(x)+\mathrm{i}\sin(x) $$
$$ \mathrm{e}^{-ix} = \cos(x)-\mathrm{i}\sin(x) $$

$$ \sin(x) =\frac {\mathrm{e}^{ix}-\mathrm{e}^{-ix}}{2\mathrm{i}} $$
$$ \cos(x) =\frac {\mathrm{e}^{ix}+\mathrm{e}^{-ix}}{2} $$
$$ \tan(x) = \frac {1}{\mathrm(i)} \frac {\mathrm{e}^{ix}-\mathrm{e}^{-ix}}
{\mathrm{e}^{ix}+\mathrm{e}^{-ix}} $$

####Other Equalities
$$ \sin(mx).\sin(nx) = \frac{1}{2} [\cos((m-n)x)-cos((m+n)x)] $$

$$ \sin(mx).\cos(nx) = \frac{1}{2}[sin((m-n)x)+\sin((m+n)x)] $$

$$ \cos(mx).\cos(nx) = \frac{1}{2} [\cos((m-n)x)+cos((m+n)x)] $$

##Limit
####Existance
Limit exists $\iff$ left-hand and right-hand limits exists and
$\lim\limits_{x \to a^-}f(x) = \lim\limits_{x \to a^+}f(x)$.

####Properties
Let,
$$ \lim\limits_{x \to c}f(x) = L  $$
$$ and $$
$$ \lim\limits_{x \to c}g(x) = M $$

Then,

1) Summation Rule: $\lim\limits_{x \to c}(f(x)+g(x))=L+M$

2) Difference Rule: $\lim\limits_{x \to c}(f(x)+g(x))=L+M$

3) Product Rule: $\lim\limits_{x \to c}(f(x).g(x))=L.M$

4) Constant Multiplication Rule: $\lim\limits_{x \to c}k.f(x)=k.L$

5) Quotient Rule: $\lim\limits_{x \to c}(\frac {f(x)}{g(x)})=\frac {L}{M}$

6) Power Rule: $\lim\limits_{x \to c}f(x)^{\frac {r}{s}}=L^{\frac {r}{s}}$

####Limits of Common Functions
$$ \lim\limits_{\theta \to 0}\frac{\sin(\theta)}{\theta} = 1 $$

$$ \lim\limits_{x \to 0}\frac{ln(1+c.x)}{x} = c $$

$$ \lim\limits_{x \to 0}\frac{\cos(x)-1}{x} = 0 $$

$$ \lim\limits_{x \to 0}\frac{\sin(x)}{x} = 1 $$


##Logarithms
1) $\log MN) = \log(M) + \log(N)$

2) $\log(\frac{M}{N}) = \log(M) - \log(N)$

3) $\log(M^k) = k \log(M)  \quad \quad   ((\log(M^k) \neq (\log(M))^k$)

4) $\log_b(M) = \frac{\log(M)}{\log(b)}$

##Differentiation
####Differentiation Properties
Let $u$ and $v$ are functions, and $c$ is constant.

$$ (c)' = 0 $$

$$ (x)' = 1 $$

$$ (u + v)' = u' + v' $$

$$ (cu)' = cu' $$

$$ (uv)' = u'v + uv' $$

$$ (\frac{u}{v})' = \frac {u'v-uv'}{v^2} $$

$$ (\frac{c}{u})' = \frac{-cu'}{v^2} $$

####Differentiation Table
$$ (x^n)' = nx^{n-1}$$

$$ (u^n)' = nu^{n-1}u' $$

$$ (e^u) = e^u u' $$



$$ (a^u)' = a^u \ln(a) u' $$

$$ (u^v)' = v u^{v-1}u' + \ln(u) u^v v' $$

$$ (log_a u)' = \log_a(e) \frac{u'}{u} = \frac{u'}{u\ln(a)} $$

$$ (\ln(u))' = \frac {u'}{u} $$

####Derivative of Trigonometric Functions
$$ (\sin(u))' = \cos(u)u' $$

$$ (\cos(u))' = -\sin(u)u' $$

$$ (\tan(u))' = \sec^2(u)u' = \frac{1}{\cos^2(u)}u' $$

$$ (\cot(u))' = -\csc^2(u)u' = -\frac{1}{\sin^2(u)}u' $$

$$ (\sec(u))' = \sec(u)\tan(u)u' $$

$$ (\csc(u))' = -\csc(u)\cot(u)u' $$


####Derivative of Inverse Functions
$$ (\arcsin(u))' = \frac{u'}{\sqrt{1-u^2}} $$

$$ (\arccos(u))' = \frac{-u'}{\sqrt{1-u^2}} $$

$$ (\arctan(u))' = \frac{u'}{1+u^2} $$

$$ (arccot(u))' = -\frac{u'}{1+u^2} $$

$$ (arcsec(u))' = \frac{u'}{|u|\sqrt{u^2-1}} $$

$$ (arccsc(u))' = \frac{-u'}{|u|\sqrt{u^2-1}} $$

##Integral
#####Table of Integrals
$$ \int (x^k)dx = \frac{x^{k+1}}{k+1} + c $$

$$ \int (\mathrm{e^x})dx = \mathrm{e^x} + c $$

$$ \int (\mathrm{a^x})dx = \frac{\mathrm{a^x}}{\ln(a)} + c $$

$$ \int \frac{1}{x}dx = \ln(|x|) + c$$


####Trigonometric Integrals
$$ \int \cos^n(x)dx =\frac{1}{n} \sin^{n-1}(x) + c $$

$$ \int \sin^n(x)dx = -\frac{1}{n}\cos^{n-1}(x) + c $$

$$ \int \tan^n(x)dx = \ln|\sec(x)| + c = \frac{1}{n-1}\tan^{n-1}(x) - \int \tan^{n-2}(x)dx $$

$$ \int \cot^n(x)dx = \ln|\sin(x)| + c = \frac{-1}{n-1}\cot^{n-1}(x) - \int \cot^{n-2}(x)dx $$

$$ \int \sec^n(x)dx = \ln|\sec(x)+\tan(x)| + c =\frac{1}{n-1}\sec^{n-2}(x)\tan(x) +\frac{n-2}{n-1}\int \sec^{n-2}(x)dx $$

$$ \int \csc^n(x)dx = \ln|\csc(x)-\tan(x)| + c = \frac{-1}{n-1}\csc^{n-2}(x)\cot(x) +\frac{n-2}{n-1}\int \csc^{n-2}(x)dx  $$

$$ \int \sec(x)\tan(x)dx = \sec(x) + c $$

$$ \int \csc(x)\cot(x)dx = -\csc(x) + c $$

$$ \int \sec^2(x)dx =  \int \frac{1}{\cos^2(x)}dx = \tan(x) + c $$

$$ \int \csc^2(x)dx = \int \frac{1}{\sin^2(x)}dx =-\cot(x) + c $$

$$ \int \cosh(x)dx = \sinh(x) + c$$

$$ \int \sinh(x)dx = \cosh(x) + c$$


####Inverse Trigonometric Integrals


$$ \int \frac {1}{\sqrt{a^2-u^2}}du = \arcsin(\frac{u}{a}) + c = -\arccos(\frac{u}{a}) + c  $$

$$ \int \frac {1}{a^2+u^2}du = \frac{1}{a}\arctan(\frac{u}{a}) + c = -\frac{1}{a}\mathrm{arccot(\frac{u}{a})} + c $$

$$ \int \frac {1}{u\sqrt{u^2-a^2}}du = \frac{1}{a}\mathrm{arcsec(\frac{|u|}{a})} + c = -\frac{1}{a}\mathrm{arccsc(\frac{|u|}{a})} + c $$
