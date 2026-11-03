Samuel Nankervis
October 26th, 2026
Math 4400, Homework 5
Dr. Han

$$\begin{aligned} &\textbf{4.1 Problem 3. } \text{Let } f(x) = 0 \text{ for } x \le 0, \text{ and } f(x) = 1 - \cos x \text{ for } x \ge 0. \text{ Is } f \text{ differentiable at } x = 0?\end{aligned}$$
To show that $f(x)$ is differentiable, we mush show that the limit, $\lim_{h \to 0} \frac{f(0+h)-f(0)}{h}$ exists. $\lim_{h \to 0^+} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0^+} \frac{1-\cos(h)-(1-\cos(0))}{h} = \lim_{h \to 0^+} \frac{1-\cos(h)}{h}$. 
Using L'Hôpital's rule, we see that,
$\lim_{h \to 0^+} \frac{1-\cos(h)}{h} =\lim_{h \to 0^+} \frac{\frac{d}{dh}(1-\cos(h))}{\frac{d}{dh}(h)} = \lim_{h \to 0^+}\frac{\sin(h)}{1} = \lim_{h \to 0^+}\sin(h) = 0.$ 
so $\frac{-\cos(h)+\cos(-h)}{2h} = \frac{-\cos(h)+\cos(h)}{2h} = \frac{0-0}{2h} = 0$.
$\lim_{h \to 0^-} \frac{f(0+h)-f(0)}{h} = \frac{0}{h} = 0$. 
Because the limit is the same coming from the right hand side and the left hand side, the limit at $x = 0$ exists, and therefore the function is differentiable at $x = 0$.
$$\begin{aligned} &\textbf{4.1 Problem 5.} \text{ Let } f(x) = A + Bx + x\vert{}x\vert{}^{p-1}g(x) \text{ where } g \text{ is a continuous function with } g(0) \neq 0. \\ &\text{For what values of } p > 0 \text{ is } f \text{ differentiable at } x = 0? \text{ If } f \text{ is differentiable at } x = 0, \\ &\text{what is } f'(0)? \text{ The answer depends on the value of } p. \end{aligned}$$
for $f(x)$ to be differentiable at $x=0$, the limit, $\lim_{h \to 0} \frac{f(0+h)-f(0)}{h}$ must exist, and therefore, 
$\lim_{h \to 0^+} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0^-} \frac{f(0+h)-f(0)}{h}$.
$\lim_{h \to 0^+} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0^-} \frac{f(0+h)-f(0)}{h} \implies$
$\lim_{h \to 0^+} \frac{A+Bh+h\vert{}h\vert{}^{p-1}g(h)-A}{h} = \lim_{h \to 0^-} \frac{A+Bh+h\vert{}h\vert{}^{p-1}g(h)-A}{h} \implies$
$\lim_{h \to 0^+} \frac{Bh+h\vert{}h\vert{}^{p-1}g(h)}{h} = \lim_{h \to 0^-} \frac{Bh+h\vert{}h\vert{}^{p-1}g(h)}{h} \implies$
$\lim_{h \to 0^+} \frac{h(B+\vert{}h\vert{}^{p-1}g(h))}{h} = \lim_{h \to 0^-} \frac{h(B+\vert{}h\vert{}^{p-1}g(h))}{h} \implies$
$\lim_{h \to 0^+} B+\vert{}h\vert{}^{p-1}g(h) = \lim_{h \to 0^-} B+\vert{}h\vert{}^{p-1}g(h)$
The limit of a constant is that constant, so $B$ has no impact on if $f$ is differentiable.
We have three cases for $p$.
Case 1, $p>1$:
If $p >1$, then $p-1>0$,  and $\lim_{ h \to 0 }\vert{}h\vert{}^{p-1}g(x) = 0$
Case 2, $p<1$:
If $p<1$, then $p-1<0$,  and $\lim_{ h \to 0 }\vert{}h\vert{}^{p-1}g(x)$ diverges to $-\infty$ for the left limit and $\infty$ for the right limit.
Case 3, $p=1$:
If $p=1$, then $p-1=0$,  and $\lim_{ h \to 0 }\vert{}h\vert{}^{p-1}g(x) = \lim_{ h \to 0 }1g(x)=g(x)$ 
Therefore, $f$ is differentiable for all $p \ge 1$.

When $f$ is differentiable with $p\ge 1$, we need to find the value of $f'(0)$.
$f'(0) = \lim_{h \to 0} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0} B+\vert{}h\vert{}^{p-1}g(h)$ as shown earlier. 
If $p>1$, then $\lim_{h \to 0} B+\vert{}h\vert{}^{p-1}g(h) = B$
If $p=1$, then $\lim_{h \to 0} B+\vert{}h\vert{}^{p-1}g(h) =B + g(0)$

$$\begin{aligned} &\textbf{4.1 Problem 7.} \text{ Let } f \text{ be differentiable at } x = a. \text{ Find} \\ &\hspace{3.5cm} \lim_{h \to 0} \frac{f(a+h) - f(a-h)}{2h}. \\ &\text{How do you interpret these quotients in terms of slopes of secant lines to the graph of } f? \end{aligned}$$
First we can split the fraction into two parts:
$\lim_{h \to 0} \frac{f(a+h) - f(a-h)}{2h} = \lim_{h \to 0} \frac{f(a+h) }{2h} - \frac{f(a-h)}{2h}$
We can then add and subtract $f(a)$.
$\lim_{h \to 0} \frac{f(a+h) }{2h} - \frac{f(a-h)}{2h} = \lim_{h \to 0} \frac{f(a+h)-f(a) }{2h} - \frac{f(a-h)-f(a)}{2h}$
We can also factor out $\frac{1}{2}$.
$\lim_{h \to 0} \frac{f(a+h)-f(a) }{2h} - \frac{f(a-h)-f(a)}{2h} = \frac{1}{2}(\lim_{h \to 0} \frac{f(a+h)-f(a) }{h} + \lim_{h \to 0} \frac{f(a-h)-f(a)}{-h})$
The first fraction is equal to $f'(a)$, because $f$ is differentiable at $x=a$.
The second fraction can be rewritten substituting $k=-h$ for $h$ in the limit.
$\lim_{h \to 0} \frac{f(a-h)-f(a)}{-h} =\lim_{k \to 0} \frac{f(a+k)-f(a)}{k}$.
The second fraction is also equal to $f'(a)$, because $f$ is differentiable at $x=a$.
$\frac{1}{2}\left( \lim_{h \to 0} \frac{f(a+h)-f(a) }{h} + \lim_{h \to 0} \frac{f(a-h)-f(a)}{-h} \right) = \frac{1}{2}(f'(a)+f'(a)) = f'(a)$.

Consider the points $A$ and $B$ where $A = (a+h, f(a+h))$, and $B = (a-h,f(a-h))$. Both points are symmetrically separated by the line $x=a$. The slope of the line between these two points is equal to $\frac{\Delta y}{\Delta x} = \frac{f(a+h)-f(a-h)}{a+h-(a-h)} = \frac{f(a+h)-f(a-h)}{2h}$. As $h$ approaches $0$, the distance between these points goes to $0$ and we will find the slope of $f(x)$ at $x=a$.

$$\begin{aligned} &\textbf{Problem 1.} \quad f(x) = \begin{cases} 2x + 3 & \text{if } x \ge 1 \\ ax^2 + bx & \text{if } x < 1 \end{cases} \\ &\text{Find } a, b \text{ such that } f \text{ is differentiable at } x = 1. \end{aligned}$$
For  $f(x)$ to be differentiable at $x=1$, the function must be continuous at $x=1$ and $\lim_{h \to 0} \frac{f(1+h)-f(1)}{h}$ must exist. We will start by finding values for $a$ and $b$ such that
$\lim_{ x \to 1^+ }f(x) = \lim_{ x \to 1^- }f(x) = f(1)$. This will show that $f$ is continuous at $x=1$.
$\lim_{ x \to 1^+ }f(x) = \lim_{ x \to 1^+ }2x+3 = 2(1)+3 =5$.
$\lim_{ x \to 1^- }f(x) = \lim_{ x \to 1^- }ax^2+bx$.
$f(1) = 2(1)+3 = 5$.
We see that $\lim_{ x \to 1^- }ax^2+bx$ must equal $5$ for $f(x)$ to be continuous at $1$.
$\lim_{ x \to 1^- }ax^2+bx = 5$. Replacing $x$ with $1$, we see that:
$a+b = 5$
Next, we need to show that $\lim_{h \to 0} \frac{f(1+h)-f(1)}{h}$ exists by evaluating each one sided limit.
$\lim_{h \to 0^+} \frac{f(1+h)-f(1)}{h} = \lim_{h \to 0^+} \frac{2(1+h)+3-(2(1)+3)}{h} = \frac{2(1+h)-2}{h} = \frac{2h}{h} = 2$.
$\lim_{h \to 0^-} \frac{f(1+h)-f(1)}{h} = \lim_{h \to 0^-} \frac{a(1+h)^2+b(1+h)-5}{h} = \lim_{h \to 0^-} \frac{a(1+h)^2+b(1+h)-(a+b)}{h} = \lim_{h \to 0^-} \frac{a+2ah+ah^2+b+bh-a-b}{h} = \lim_{h \to 0^-} \frac{2ah+ah^2+bh}{h} = \lim_{h \to 0^-} \frac{h(2a+ah+b)}{h} = \lim_{h \to 0^-} 2a+ah+b$
$= 2a+b$.
For $\lim_{h \to 0} \frac{f(1+h)-f(1)}{h}$ to exist, the one sided limits must be equivalent. We know the right limit is $2$, so the left limit must also equal $2$.
$2a+b = 2$
Solving our linear equation for $b$, 
$b = 2-2a$, 
$a+(2-2a) = 5 \implies a=-3$
$b = 2-2(-3) \implies b = 8$.
Because $a$ and $b$ satisfy both equations, when $a=-3$ and $b=8$, $f(x)$ is differentiable at $x=1$.

$$\begin{aligned} &\textbf{Problem 2.} \quad f(x) = \begin{cases} x\vert{}x\vert{}^{r-1} \sin\left(\frac{1}{x}\right) & \text{if } x \neq 0 \\ 0 & \text{if } x = 0 \end{cases} \\ &\text{Find } f'(0) \text{ (Hint: Three cases: } r < 1, \, r = 1, \text{ and } r > 1). \end{aligned}$$
To find $f'(0)$, we calculate $\lim_{h \to 0} \frac{f(0+h)-f(0)}{h}$. Because $r$ is unknown, we have three cases.
$r<1,r=1,r>1$
Case 1, $r<1$:
$\lim_{h \to 0} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0} \frac{h\vert{}h\vert{}^{r-1}\sin\left( \frac{1}{h} \right)-0}{h} = \lim_{h \to 0} \vert{}h\vert{}^{r-1}\sin\left( \frac{1}{h} \right)$. $\sin\left( \frac{1}{h} \right)$ will be between $(-1,1)$ for any given $h$ as $h \to 0$. $\lim_{ h \to 0 } \vert{}h\vert{}^{r-1} = \infty$. Because $\lim_{h \to 0} \sin\left( \frac{1}{h} \right)$ could be negative or positive for any given value of $h$ as $h \to 0$, it is not possible to determine if $\lim_{h \to 0} \vert{}h\vert{}^{r-1}\sin\left( \frac{1}{h} \right) = \infty$ or $-\infty$. Thus $f'(x)$ is undefined if $r<1$.
Case 2, $r=1$:
$\lim_{h \to 0} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0} \frac{h\vert{}h\vert{}^{1-1}\sin\left( \frac{1}{h} \right)-0}{h} = \lim_{h \to 0} \vert{}h\vert{}^{0}\sin\left( \frac{1}{h} \right) = \lim_{h \to 0} \sin\left( \frac{1}{h} \right)$. As discussed earlier, $\lim_{h \to 0} \sin\left( \frac{1}{h} \right)$ does not exist.
Case 3, $r>1$:
$\lim_{h \to 0} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0} \frac{h\vert{}h\vert{}^{r-1}\sin\left( \frac{1}{h} \right)-0}{h} = \lim_{h \to 0} \vert{}h\vert{}^{r-1}\sin\left( \frac{1}{h} \right)$. With $r>1$, $\lim_{ h \to 0 } \vert{}h\vert{}^{r-1} = 0$. As discussed earlier, $\sin\left( \frac{1}{h} \right)$ will be between $(-1,1)$ for any given $h$ as $h \to 0$. Multiplying these together, we see that $\lim_{h \to 0} \vert{}h\vert{}^{r-1}\sin\left( \frac{1}{h} \right) = 0$.
$$\begin{aligned} &\textbf{Problem 3.} \quad f(x) = \begin{cases} x - x^2 \sin \frac{1}{x} & \text{if } x \neq 0 \\ 0 & \text{if } x = 0. \end{cases} \\ &\text{a) Show that } f'(0) = 1. \\ &\text{b) Show that } \lim_{x \to 0} f'(x) \text{ does not exist.} \end{aligned}$$
To find $f'(0)$, we calculate $\lim_{h \to 0} \frac{f(0+h)-f(0)}{h}$. 
$\lim_{h \to 0} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0} \frac{h-h^2\sin\left( \frac{1}{h} \right)-0}{h} = \lim_{h \to 0} \frac{h(1-h\sin\left( \frac{1}{h} \right))}{h} = \lim_{h \to 0} 1-h\sin\left( \frac{1}{h} \right)$.
Because $\lim_{h \to 0} \sin\left( \frac{1}{h} \right)$ is between $(-1,1)$, $\lim_{h \to 0} h = 0$, and the limit operation does not effect constants, $\lim_{h \to 0} 1-h\sin\left( \frac{1}{h} \right) = 1$. 

$f'(x) = 1-\left( 2x\sin\left( \frac{1}{x} \right) \right)+\left( x^2\cos\left( \frac{1}{x} \right) (-\frac{1}{x^2}) \right) = 1-2x\sin\left( \frac{1}{x} \right) +\cos\left( \frac{1}{x} \right) (-\frac{ x^2}{x^2})$
$= 1-2x\sin\left( \frac{1}{x} \right) -\cos\left( \frac{1}{x} \right)$ 
$\lim_{ x \to 0 } 1-2x\sin\left( \frac{1}{x} \right) -\cos\left( \frac{1}{x} \right)$ does not exist because $\lim_{ x \to 0 } \cos\left( \frac{1}{x} \right)$ does not exist.

$$\begin{aligned} &\textbf{Problem 4.} \quad f(x) = \begin{cases} x - x^3 \sin \frac{1}{x} & \text{if } x \neq 0 \\ 0 & \text{if } x = 0. \end{cases} \\ &\text{a) Show that } f'(0) = 1. \\ &\text{b) Show that } \lim_{x \to 0} f'(x) = f'(0). \end{aligned}$$
To find $f'(0)$, we calculate $\lim_{h \to 0} \frac{f(0+h)-f(0)}{h}$. 
$\lim_{h \to 0} \frac{f(0+h)-f(0)}{h} = \lim_{h \to 0} \frac{h-h^3\sin\left( \frac{1}{h} \right)-0}{h} = \lim_{h \to 0} \frac{h(1-h^2\sin\left( \frac{1}{h} \right))}{h} = \lim_{h \to 0} 1-h^2\sin\left( \frac{1}{h} \right) = 1$.
Because $\lim_{h \to 0} \sin\left( \frac{1}{h} \right)$ is between $(-1,1)$, $\lim_{h \to 0} h^2 = 0$, and the limit operation does not effect constants, $\lim_{h \to 0} 1-h^2\sin\left( \frac{1}{h} \right) = 1$. 

$f'(x) = 1-\left( 3x^2\sin\left( \frac{1}{x} \right) \right)+\left( x^3\cos\left( \frac{1}{x} \right)\left( -\frac{1}{x^2} \right) \right) = 1-\left( 3x^2\sin\left( \frac{1}{x} \right) \right)-\left( x\cos\left( \frac{1}{x} \right) \right)$.
$\lim_{ x \to 0 } 1-\left( 3x^2\sin\left( \frac{1}{x} \right) \right)-\left( x\cos\left( \frac{1}{x} \right) \right) = 1- \lim_{ x \to 0 } \left( 3x^2\sin\left( \frac{1}{x} \right) \right) -\lim_{ x \to 0 } \left( x\cos\left( \frac{1}{x} \right) \right)$.
The limits $\lim_{h \to 0} \sin\left( \frac{1}{x} \right)$ and $\lim_{ x \to 0 } \left(\cos\left( \frac{1}{x} \right) \right)$ are between $(-1,1)$.
The limits $\lim_{x \to 0} 3x^2 = 0$ and $\lim_{x \to 0} x = 0$.
So $1- \lim_{ x \to 0 } \left( 3x^2\sin\left( \frac{1}{x} \right) \right) -\lim_{ x \to 0 } \left( x\cos\left( \frac{1}{x} \right) \right) = 1$. 

