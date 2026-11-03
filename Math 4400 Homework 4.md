Samuel Nankervis
October 12th, 2026
Math 4400, Homework 4
Dr. Han

Problems from 3.1:

1. Let $a$ be a limit point of $D(f)$ and suppose that $\lim_{x \to a} f(x) = L$. Show that $\lim_{x \to a} \vert{}f(x)\vert{} = \vert{}L\vert{}$.

Let $\epsilon$ be an arbitrary number greater than zero.
$\lim_{x \to a} f(x) = L$ implies that there exists a $\delta>0$ such that for all $x\in D(f)$, $0 < \vert{}x-a\vert{}<\delta$. This implies that $\vert{}f(x)-L\vert{}<\epsilon$. 
Applying the reverse triangle inequality, we see that $\vert{}\vert{}f(x)\vert{}-\vert{}L\vert{}\vert{} \le\vert{}f(x)-L\vert{}<\epsilon$.
Thus, $0 \le \vert{}x-a\vert{}<\delta \implies \vert{}\vert{}f(x)\vert{}-\vert{}L\vert{}\vert{}<\epsilon$. So by definition $\lim_{x \to a} \vert{}f(x)\vert{} = \vert{}L\vert{}$.

9. Give an example where $\lim_{x \to a} f(x)$ exists and $\lim_{x \to a} f(x)g(x)$ exists, but $\lim_{x \to a} g(x)$ does not exist.
	
	Let $f(x) = 0x$. We now prove that $\lim_{ x \to 0 }f(x) =0$ .
	We choose $\delta =\epsilon$.
	Let $\epsilon$ be arbitrary and $\epsilon>0$. If $0<\vert{}x-0\vert{}<\delta$, then $\vert{}0-0\vert{} < \vert{}x-0\vert{}<\delta = \epsilon$. 
	Thus $\lim_{ x \to 0 }f(x) =0$
	
	Let $g(x) = (-1)^x$. We now prove that $\lim_{ x \to 0 }g(x)$ does not exist. We know that if two different subsequences of a set converge to two different limits, then the limit of the whole function does not exist. Consider the subsequences $g_{even}(x) = (-1)^{2x}$ and $g_{odd}(x) = (-1)^{2x+1}$. $g_{even}(x) = 1$, so $\lim_{ x \to 0 }g_{even}(x) = 1$. $g_{odd}(x) = -1$, so $\lim_{ x \to 0 }g_{odd}(x) = -1$. Because the two subsequences of $g(x)$ converge to two different limits, the limit of $g(x)$ does not exist.
	
	Consider $f(x)g(x)$. $f(x)g(x) = 0\times(-1)^x = 0$ As shown earlier, the limit of a constant function is that constant. So $\lim_{ x \to 0 }f(x)g(x) = 0$. Thus it is possible that $\lim_{x \to a} f(x)$ exists and $\lim_{x \to a} f(x)g(x)$ exists, but $\lim_{x \to a} g(x)$ does not exist.


Problems from 3.3:

1.Let $f$ be continuous on $I = [a, b]$ with $f(x) > 0$ for all $x \in I$. Show that there is a constant $c > 0$ such that $f(x) \ge c > 0$ for all $x \in I$. Is the result still true if we allow $I$ to be half-open, $I = [a, b)$?

$f(x)$ is continuous on $[a,b]$, by Theorem 3.6, there exists a minimizer $x_{*}\in [a,b]$ such that $f(x_{*})\le f(x)$ for all $x \in I$, and $f(x_{*})$ is the minimum value of the range of $f(x)$ in the interval $[a,b]$ 
Because $x_{*}$ is a constant, we can let $c = x_{*}$. Because $f(x) > 0$ for all $x$, and $f(x_{*})$ is the minimum of the range of the function under the interval $[a,b]$, we see that $f(x) \ge c > 0$. 

The statement is not true when the interval is not bounded. This is because we can no longer assume that f(x) has a minimizer, $x_{*} \in I$. 
Consider the function $f(x) = x$ on the interval $(0,1]$. 
While $f(x)$ is strictly greater than zero for all $x \in (0,1]$, There does not exist a minimizer for the function on this interval, so we know of no definite value greater than $0$ that is also the minimum of the function.

3. Show that $f(x) = x^2$ is not uniformly continuous on $\mathbb{R}$.
    
	Analysis: $\vert{}f(x)-f(y)\vert{} = \vert{}x^2-y^2\vert{} = \vert{}x+y\vert{}\vert{}x-y\vert{}$.
	
	Proof: There exists a single fixed $\epsilon_{0} = 1$ for every $\delta$, there exist $x$ and $y$ with $\vert{}x-y\vert{}<\delta$ and $\vert{}f(x)-f(y)\vert{}\ge \epsilon_{0}$. 
	Let $x_{n} = n+\frac{1}{n}$ and $y_{n} = n$. Then $\vert{}x_{n}-y_{n}\vert{} = \frac{1}{n} \to 0$.
	$\vert{}x_{n}^2-y_{n}^2\vert{} = \vert{}n^2 + 2+\frac{1}{n^2}-n^2\vert{}= \vert{}2+\frac{1}{n^2}\vert{} \to 2>1$.
	Thus $𝑓(𝑥) = 𝑥^2$ is not uniformly continuous on $\mathbb{R}$.
    
4. By making direct estimates, show that $f(x) = x/(1 + x^2)$ is uniformly continuous on $\mathbb{R}$.

Analysis:
For $\epsilon > 0$, We need to choose $\delta$ such that if $\vert{}x-y\vert{}<\delta$, then $\vert{} \frac{x}{1+x^2}-\frac{y}{1+y^2}\vert{}<\epsilon$.
$\vert{} \frac{x}{1+x^2}-\frac{y}{1+y^2}\vert{} = \vert{} \frac{x(1+y^2)-y(1+x^2)}{(1+x^2)(1+y^2)}\vert{} = \frac{\vert{}1-xy\vert{}}{(1+x^2)(1+y^2)}\vert{}y-x\vert{}$.
We need to find an upper bound for $\frac{\vert{}1-xy\vert{}}{(1+x^2)(1+y^2)}$.  
Considering the numerator, $\vert{}1-xy\vert{}\le 1+ \vert{}xy\vert{}$. 
For the denominator, $(1+x^2)(1+y^2) = 1 + x^2 + y^2 + x^2y^2 \ge 1 + 2\vert{}xy\vert{} + x^2y^2 = (1 + \vert{}xy\vert{})^2$.
So $\frac{\vert{}1-xy\vert{}}{(1+x^2)(1+y^2)} \le \frac{1+\vert{}xy\vert{}}{(1+\vert xy\vert)^2} = \frac{1}{(1+ \vert xy\vert)} \le 1$. 
Therefore, $\vert{} \frac{x}{1+x^2}-\frac{y}{1+y^2}\vert{}<\epsilon \Longleftrightarrow (1)\vert{}x-y\vert{} < \epsilon \Longleftrightarrow \vert{}x-y\vert{} < \epsilon$.
So we choose $\delta =\epsilon$.

Proof:
Let $\epsilon$ be arbitrary.
If $0 < \vert{}x-y\vert{}<\delta$, then $\vert{} \frac{x}{1+x^2}-\frac{y}{1+y^2}\vert{} = \frac{\vert{}1-xy\vert{}}{(1+x^2)(1+y^2)}\vert{}y-x\vert{} \le \vert{}x-y\vert{} < \delta = \epsilon$.
Thus, $f(x) = x/(1 + x^2)$ is uniformly continuous on $\mathbb{R}$.

**Problem 1.** Find the set of limit points for each set.

1. $A = (0, 2]$.
    
    0 is a limit point to the set because we can choose $x_{n} = 0 + \frac{1}{n}$, which is in $A$ for all $n$. This sequence converges to 0, thus 0 is a limit point, and the set of limit points in $A$ is $[0,2]$.
    
2. $B = \left\{ -1, 2, -\frac{3}{2}, \frac{8}{5}, \dots, \frac{(-1)^n 2n}{n+1}, \dots \right\}$.
    
    The positive values of the sequence (with $n$ being even) can be written as $\frac{4n}{2n+1}\in B$. This converges to $\frac{4}{2} =2$. 
    Similarly, the negative values of the sequence (with $n$ being odd) can be written as $\frac{-2(2n+1)}{(2n+1)+1}\in B$. This converges to $\frac{-4}{2} =-2$. 
    Because we can choose a small enough $\epsilon >0$ such that $-2 + \epsilon$ and $2 - \epsilon$ contains only a finite number of points, there does not exist another limit point within the sequence. 
    
3. $C = \text{all irrational numbers in } (\sqrt{3}, 8)$.
    
    Because the irrationals are dense in $(\sqrt{3}, 8)$, There exists a sequence $x_{n} \in \mathbb{R}-\mathbb{Q}\cap(\sqrt{3},8)$ that converges to $a$ with $a \in [\sqrt{3}, 8]$. Thus the limit point is $[\sqrt{3}, 8]$.
    
4. $D = \text{all rational numbers in } (-\sqrt{2}, \sqrt{2})$.
    
    Because the rationals are dense in $(-\sqrt{2}, \sqrt{2})$, There exists a sequence $x_{n} \in \mathbb{Q}\cap(-\sqrt{2}, \sqrt{2})$ that converges to $a$ with $a \in [-\sqrt{2}, \sqrt{2}]$. Thus the limit point is $[-\sqrt{2}, \sqrt{2}]$.
    
5. $E = (2, 3) \cup (3, 9)$.
    
    The set of limit points in $(2,3)$ is $[2,3]$. 
    The set of limit points in $(3,9)$ is $[3,9]$. 
    Thus, the set of limit points in $(2, 3) \cup (3, 9)$ is $[2,3] \cup [3,9] \implies [2,9]$.

**Problem 2.** Use the $(\epsilon, \delta)$ formulation of the limit to show that

$$\lim_{x \to 0} \sqrt{x + \frac{1}{3}} = \sqrt{\frac{1}{3}}$$
Analysis: For $\epsilon > 0$, We need to choose $\delta$ such that if $0 < \vert{}x-0\vert{}<\delta$, then $\vert{}\sqrt{x+\frac{1}{3}}-\sqrt{\frac{1}{3}}\vert{}<\epsilon$. 
$\vert{}\sqrt{x+\frac{1}{3}}-\sqrt{\frac{1}{3}}\vert{}<\epsilon \Longleftrightarrow \vert{}\frac{\left( \sqrt{x+\frac{1}{3}}-\sqrt{\frac{1}{3}} \right)\left( \sqrt{x+\frac{1}{3}}+\sqrt{\frac{1}{3}} \right)}{\sqrt{x+\frac{1}{3}}+\sqrt{\frac{1}{3}}}\vert{}<\epsilon\Longleftrightarrow\vert{}\frac{x+\frac{1}{3}-\frac{1}{3}}{\sqrt{x+\frac{1}{3}}+\sqrt{\frac{1}{3}}}\vert{}<\epsilon\Longleftrightarrow\frac{\vert{}x\vert{}}{\sqrt{x+\frac{1}{3}}+\sqrt{\frac{1}{3}}}<\epsilon$.
Because $\sqrt{x+\frac{1}{3}}+\sqrt{\frac{1}{3}}\ge \frac{1}{\sqrt{3}}$ for all possible values of $x$, $\frac{\vert{}x\vert{}}{\sqrt{x+\frac{1}{3}}+\sqrt{\frac{1}{3}}}\le \frac{\vert{}x\vert{}}{\frac{1}{\sqrt{3}}}=\sqrt{3}\vert{}x-0\vert{}$. If $\vert{}x-0\vert{}< \frac{\epsilon}{\sqrt{3}}$, Then the inequality will be satisfied. We choose $\delta = \frac{\epsilon}{\sqrt{3}}$.
Let $\epsilon$ be arbitrary.
If $0 < \vert{}x-0\vert{}<\delta$, then $\vert{}\sqrt{x+\frac{1}{3}}-\sqrt{\frac{1}{3}}\vert{} =\frac{\vert{}x\vert}{\sqrt{x+\frac{1}{3}}+\sqrt{\frac{1}{3}}} {}\le\sqrt{3}\vert{}x-0\vert{}<\sqrt{3} \frac{\epsilon}{\sqrt{3}}=\epsilon$.
Thus $\lim_{x \to 0} \sqrt{x + \frac{1}{3}} = \sqrt{\frac{1}{3}}$.


**Problem 3.** Show that $f(x) = \frac{1}{1+x^4}$ is uniformly continuous on $\mathbb{R}$.

Analysis: For $\epsilon > 0$, We need to choose $\delta$ such that if $\vert{}x-y\vert{}<\delta$, then $\vert{} \frac{1}{1+x^4}-\frac{1}{1+y^4}\vert{}<\epsilon$. 
$\vert{} \frac{1}{1+x^4}-\frac{1}{1+y^4}\vert{} = \vert{} \frac{(1+y^4) - (1+x^4)}{(1+x^4)(1+y^4)} \vert{} = \vert{} \frac{y^4 - x^4}{(1+y^4+x^4+y^4x^4)} \vert{} =  \frac{(x^2+y^2)\vert{}(x+y)\vert{}}{(1+y^4+x^4+y^4x^4)}  \vert{}x-y\vert{}$.
We need to find an upper bound for $\frac{(x^2+y^2)\vert{}(x+y)\vert{}}{(1+y^4+x^4+y^4x^4)}$.  
Using the Cauchy-Schwarz Inequality on the numerator, we see that:
$\vert{}x+y\vert{} \le \sqrt{1^2+1^2}\sqrt{x^2+y^2} = \sqrt{2}\sqrt{x^2+y^2}$
$\sqrt{2}(x^2+y^2)\sqrt{x^2+y^2} = \sqrt{2}(x^2+y^2)^{3/2} \ge (x^2+y^2)\vert{}(x+y)\vert{}$.

I'm not sure how to find an upper bound for that problem.

**Problem 4.** Show that $f(x) = \frac{1}{x}$ is uniformly continuous on $[1, \infty)$.

Analysis: For $\epsilon > 0$, We need to choose $\delta$ such that if $\vert{}x-y\vert{}<\delta$, then $\vert{} \frac{1}{x}-\frac{1}{y}\vert{}<\epsilon$.
$\vert{} \frac{1}{x}-\frac{1}{y}\vert{} = \vert{} \frac{y-x}{xy}\vert{} = \frac{\vert{}x-y\vert{}}{xy}$.
Because $y \in [1, \infty)$, and $x \in [1, \infty)$, $xy \ge 1$. So $\frac{\vert{}x-y\vert{}}{xy} \le \frac{\vert{}x-y\vert{}}{1} = \vert{}x-y\vert{}$. So we choose $\delta = \epsilon$. 

Proof:
Let $\epsilon$ be arbitrary.
If $0 < \vert{}x-y\vert{}<\delta$ for all $y \in [1, \infty)$ and $x \in [1, \infty)$, then $\vert{} \frac{1}{x}-\frac{1}{y}\vert{} = \vert{} \frac{y-x}{xy}\vert{} \le \vert{}x-y\vert{} < \delta = \epsilon$.
Thus, $f(x) = \frac{1}{x}$ is uniformly continuous on $[1, \infty)$.

**Problem 5.** Show that $f(x) = \frac{1}{x-8}$ is not uniformly continuous on $[2, 8)$.

I didn't have time to do this proof. 