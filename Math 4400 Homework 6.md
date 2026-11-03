Samuel Nankervis
October 30th, 2026
Math 4400, Homework 6
Dr. Han

2. Let $f(x) = 1/x + 2\sqrt{x + 1}$ for $x > 0$.

a) Show that $f(x) > f(2)$ for $x \ge 2$ and that $f(x) > f(1)$ for $0 < x \le 1$.

First, we calculate $f(2)$. 
$f(2)=1/2 + 2\sqrt{2 + 1} = \frac{1}{2}+2\sqrt{3}$.
Next, we calculate $f'(x)$.
$f'(x) = -\frac{1}{x^2}+\frac{1}{\sqrt{ x+1 }}$.
If $x \ge 2$ then $x^4> x+1\implies x^2> \sqrt{ x+1 }$.
Taking the reciprocal of both sides, we see that 
$x^2> \sqrt{ x+1 } \implies \frac{1}{x^2}< \frac{1}{\sqrt{ x+1 }} \implies 0 < \frac{1}{\sqrt{ x+1 }}-\frac{1}{ x^2}$.
Thus $f'(x)\ge 0$ when $x \ge 2$.  and $f(x)$ is increasing when $x\ge 2$.
Because $f(x)$ is increasing when $x\ge 2$, $f(x)\ge f(2)$ when $x\ge 2$.

First, we calculate $f(1)$. 
$f(1) = \frac{1}{1}+2\sqrt{ 1+1 } = 1+2\sqrt{ 2 }$.
If $0<x\le 1$, then $x^4< x+1\implies x^2< \sqrt{ x+1 }$
Taking the reciprocal of both sides, we see that
$x^2< \sqrt{ x+1 } \implies \frac{1}{x^2}> \frac{1}{\sqrt{ x+1 }} \implies 0 > \frac{1}{\sqrt{ x+1 }}-\frac{1}{ x^2}$.
Thus $f'(x)\le 0$ when $0<x\le 1$.  and $f(x)$ is decreasing when $0<x\le 1$.
Because $f(x)$ is decreasing when $0<x\le 1$, $f(x)\ge f(1)$ when $0<x\le 1$.

6. Suppose that $f$ is differentiable on $\mathbb{R}$ and that $f'(x) \ge c > 0$ for all $x$.
a) Show that for $x > 0$, $f(x) \ge f(0) + cx$.

If $f$ is differentiable on $\mathbb{R}$, then this implies that $f$ is continuous and differentiable on $[0,x]$.
We can apply the mean value theorem to this interval. There exists some $\theta \in [0,x]$ such that:
If $x>0$, then $f(x)-f(0)=f'(\theta)(x-0) \implies$
$f(x)=f'(\theta)(x-0)+f(0) \implies$
$f(x)=f(0)+f'(\theta)x$
If $f'(x) \ge c > 0$, it follows that $f'(\theta) \ge c > 0$.
Therefore,
$f(x)\ge f(0)+cx$.

b) Show that for $x < 0$, $f(x) \le f(0) + cx$.

If $f$ is differentiable on $\mathbb{R}$, then this implies that $f$ is continuous and differentiable on $[x,0]$.
We can apply the mean value theorem to this interval. There exists some $\theta \in [x,0]$ such that:
If $0>x$, then $f(0)-f(x)=f'(\theta)(0-x) \implies$
$-f(x) = -f(0)-f'(\theta)x \implies$
$f(x) = f(0)+f'(\theta)x$
If $f'(x) \ge c > 0$, it follows that $f'(\theta) \ge c > 0$.
Therefore,
$f(x) \le f(0)+cx$.
The inequality is different from part a, because $x<0$, so multiplying a smaller number by a negative will make their product larger.

**Problem 1:** Let $u(t)$ and $v(t)$ be $C^1$ function on $R$, and suppose that they solve the system of differential equations:

$$\begin{aligned} u' &= v \\ v' &= -\sin u \end{aligned}$$

Set $K(t) = \frac{v^2(t)}{2} - \cos(u(t))$. Prove that $K(t)$ is constant(Hint: Show that $K'(t) = 0$).

I haven't taken differential equations, so hopefully I did this right.

First we find $\frac{d}{dt}(K(t)) =K'(t)$. 
$K'(t) = \frac{d}{dt}\left( \frac{v^2(t)}{2} \right)-\frac{d}{dt}(\cos(u(t)))$.
$\frac{d}{dt}\left( \frac{v^2(t)}{2} \right) = \frac{1}{2}2v(t)v'(t) =v(t)v'(t)$.
$\frac{d}{dt}(\cos(u(t))) =-\sin(u(t))u'(t)$.
So, $K'(t) = v(t)v'(t) - (-\sin(u(t))u'(t)) = v(t)v'(t) + \sin(u(t))u'(t)$.
Substituting in $u' = v$ and $v' = -\sin(u)$ into $K'(t)$,
$K'(t)=v(t)(-\sin(u)) + \sin(u(t))v = -\sin(u(t))v + \sin(u(t))v =0$.

Because $K'(t)=0$, $K(t)$ must be constant. 

