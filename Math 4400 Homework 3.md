Samuel Nankervis
October 5th, 2026
Math 4400, Homework 3
Dr. Han
Score: 7/10

Problems from page 50:

4. Let the sequence $\{a_n\}$ be given recursively by
    $a_{n+1} = \frac{1}{4} + a_n^2, \quad a_1 = 0.$
    Show that the sequence $\{a_n\}$ converges and find the limit.
    
    First, we must find a proposed limit for the function. Let's replace $a_{n}$ and $a_{n+1}$ with $L$, the limit of the sequence.
    $L = \frac{1}{4}+L^2 \implies L^2-L+\frac{1}{4} = 0 \implies (2L-1)^2 = 0 \implies L = \frac{1}{2}$.
    Now that we have a proposed limit, we can try to prove that:
    The sequence {$a_n$} for all $n\ge 1$ is below $\frac{1}{2}$.
    Consider $a_{1}$. 
    $a_{1} = 0 \le \frac{1}{2}$. so the statement is true for $a_{1}$.
    We now assume that $a_{n} \le \frac{1}{2}$.
    Consider $a_{n+1}$.
    $a_{n+1} \le \frac{1}{4}+\left( \frac{1}{2} \right)^2$. 
    $\frac{1}{4}+\left( \frac{1}{2} \right)^2 = \frac{1}{2}$. 
    So $a_{n+1} \le \frac{1}{2}$, and thus, the sequence has an upper bound of $\frac{1}{2}$.
    Next, we must prove that $a_{n+1}\ge a_{n}$.
    $a_{n+1}\ge a_{n} \implies a_{n+1} - a_{n} \ge 0$.
    $a_{n+1}-a_{n} = \frac{1}{4}+a_{n}^2-a_{n} = \frac{1}{4}(2a_{n}-1)^2$. 
    For any real number, $x$, $x^2 \ge 0$, and $\frac{1}{4}x^2 \ge 0$. 
    So $a_{n+1}\ge a_{n}$ for all $n$, and the sequence is therefore monotone increasing.
    We have now shown that the sequence is both monotone increasing and bounded above.
    Thus, by Theorem 2.8, the sequence converges.
    
5. Discuss the convergence of the sequence $\{y_n\}$ where $y_1 = 1$ and, for $n \ge 1$, $y_{n+1} = \sqrt{y_n + 2}$.
	
	First, we must find a proposed limit for the function. Let's replace $y_{n}$ and $y_{n+1}$ with $L$, the limit of the sequence.
	$L = \sqrt{L+2} \implies L^2 = L+2 \implies L^2-L-2 = 0 \implies (L-2)(L+1) = 0$.
	So $L = 2$ or $L = -1$. Because $2>-1$, and $y_{n}$ is increasing, $L=2$.
	Now that we have a proposed limit, we can try to prove that:
	The sequence {$y_n$} for all $n\ge 1$ is below $2$.
	Consider $y_{1}$. $y_{1} = 1 \le 2$. So the statement is true for $y_{1}$.
	We now assume that  $y_{n}\le 2$.
	Consider $y_{n+1}$.
	$y_{n+1} = \sqrt{y_n + 2} \le \sqrt{2+2} = 2$.
	So $y_{n+1} \le 2$, and thus the sequence has an upper bound of $2$.
	Next, we must prove that $y_{n+1}\ge y_{n}$.
    $y_{n+1}\ge y_{n} \implies \sqrt{y_{n}+2} \ge y_{n}$
    We know that $y_{n}$ starts at one and is increasing, so squaring each side does not flip the inequality.
    $\sqrt{y_{n}+2} \ge y_{n} \implies y_{n} + 2 \ge y_{n}^2 \implies y_{n}^2-y_{n}-2 \le 0 \implies (y_{n}-2)(y_{n}+1)\le 0$. 
    This inequality holds for all $y_{n} \in [-1,2]$. Because $-1< y_{n} \le 2$ as shown above, we see that $y_{n+1}\ge y_{n}$ and $y_{n}$ is monotone increasing.
    We have now shown that the sequence is both monotone increasing and bounded above.
    Thus, by Theorem 2.8, the sequence converges.


Problems from homework 3:

Problem 1. If $a_1 = 2, a_{n+1} = \frac{3a_n + 5}{4}$ for $n \ge 1$, show that $\{a_n\}$ is monotone increasing and bounded above. Find the limit of $\{a_n\}$.

First, we must find a proposed limit for the function. Let's replace $a_{n}$ and $a_{n+1}$ with $L$, the limit of the sequence.
$L = \frac{3L+5}{4} \implies 4L = 3L+5 \implies L = 5$.
Now that we have a proposed limit, we can try to prove that:
The sequence {$a_n$} for all $n\ge 1$ is below $5$.
Consider $a_{1}$. 
$a_{1} = 2 \le 5$. so the statement is true for $a_{1}$.
We now assume that $a_{n} \le 5$.
Consider $a_{n+1}$.
$a_{n+1} = \frac{3a_{n}+5}{4} \le \frac{3(5)+5}{4} = \frac{20}{4} = 5$
So $a_{n+1} \le 5$ for all $n$, and $5$ is an upper bound of the set.
Next, we must prove that $a_{n+1}\ge a_{n}$.
from earlier, we know that $a_{n}\le 5 \implies 4a_{n} \le 5+3a_{n} \implies a_{n} \le \frac{5+3a_{n}}{4} \implies a_{n+1}\ge a_{n}$.
Now we can see that $a_{n}$ is monotone increasing and bounded above.


Problem 2. If $a_1 = 2, a_{n+1} = \frac{3a_n - 7}{4}$ for $n \ge 1$, show that $\{a_n\}$ is monotone decreasing and bounded below. Find the limit of $\{a_n\}$.

First, we must find a proposed limit for the function. Let's replace $a_{n}$ and $a_{n+1}$ with $L$, the limit of the sequence.
$L = \frac{3L-7}{4} \implies 4L = 3L-7 \implies L = -7$.
Now that we have a proposed limit, we can try to prove that:
The sequence {$a_n$} for all $n\ge 1$ is above $-7$.
Consider $a_{1}$. 
$a_{1} = 2 \ge 7$. so the statement is true for $a_{1}$.
We now assume that $a_{n} \ge -7$.
Consider $a_{n+1}$.
$a_{n+1} = \frac{3a_{n}-7}{4} \ge \frac{3(-7)-7}{4} = \frac{-28}{4} = -7$.
So $-7$ is a lower bound for $a_{n}$.
Next, we must prove that $a_{n+1}\le a_{n}$.
from earlier, we know that $-7 \le a_{n} \implies 3a_{n}-7 \le 4a_{n} \implies \frac{3a_{n}-7}{4}\le a_{n} \implies a_{n+1}\le a_{n}$.
Thus, the sequence is both monotone decreasing and bounded below.

Problem 3. Let $a_1 = \frac{1}{2}$ and define $a_{n+1} = a_n(2 - a_n)$ for $n \ge 1$. Show that $a_n$ converges and find the limit.

First, we must find a proposed limit for the function. Let's replace $a_{n}$ and $a_{n+1}$ with $L$, the limit of the sequence.
$L = L(2-L) \implies -L^2 +L = 0 \implies L(-L+1) =0 \implies L = 0$ or $L=1$. 
$a_{n}$ is increasing so we choose $L=1$.
Now that we have a proposed limit, we can try to prove that:
The sequence {$a_n$} for all $n\ge 1$ is below $1$.
Consider $a_{1}$. 
$a_{1} = \frac{1}{2} \le 1$. so the statement is true for $a_{1}$.
We now assume that $a_{n} \le 1$.
Consider $a_{n+1}$.
$a_{n+1} = a_{n}(2-a_{n})\le 1(2-1) = 1$.
So $1$ is an upper bound for $a_{n}$.
Next, we must prove that $a_{n+1}\ge a_{n}$.
$a_{n+1}\ge a_{n} \implies a_{n+1} - a_{n} \ge 0$.
$a_{n+1}-a_{n} = a_{n}(2-a_{n})-a_{n} = -a_{n}^2+a_{n}$.
If $a_{n}^2 \le a_{n}$ for all $n$, $a_{n+1}\ge a_{n}$
$a_{n}^2 \le a_{n}$ when $-1\le a_{n} \le 1$. We know from earlier that $\frac{1}{2}\le a_{n}\le 1$. 
Thus, $a_{n+1}\ge a_{n}$ and $a_{n}$ is monotone increasing.
Because $a_{n}$ is monotone increasing and is bounded from above, the sequence converges.

Problem 4. Determine whether each of the following statements is true or false. If it is true, prove it. If it is false, give a counterexample.

a) Let $\{a_n\}$ be a sequence. If $\{a_n\}$ converges, then $\{a_n^2\}$ converges.

The statement is true.
Consider the convergent sequence $a_n$. Because $a_{n}$ converges, there exists a limit, $L$, to the sequence $a_{n}$ such that $\lim_{ n \to \infty }a_{n} = L$.
Consider $a_{n}^2 = (a_{n})  (a_{n})$. 
$a_{n}$ converges to $L$ as $n\to \infty$, so $(a_{n})  (a_{n})$ converges to $(L)(L) = L^2$.
Because a limit exists for $a_{n}^2$, it converges.

b) Let $\{a_n\}$ be a sequence. If $\{a_n^2\}$ converges, then $\{a_n\}$ converges.

The statement is false. 
Let $a_{1} = 1$ and define $a_{n+1} = -a_{n}$. So $a_{1}^2 = 1$ and $a_{n+1}^2 = (-a_{n})^2 = a_{n}^2$. 
$a_{n+1}^2$ converges because $a_{n+1}^2 = a_{n}^2$ and $a_{n}^2 = 1$ for all $n$.
However, $a_{n}$ diverges. Consider the subsequences $a_{n\space odd}$ and $a_{n\space even}$ where each is the odd and even values of n within the sequence of $a_n$.
$a_{n\space odd +1} = -(-a_{n\space odd}) = a_{n\space odd}$ with it's first value equal to $a_{1} = 1$. So $\lim_{ n \to \infty } a_{n\space odd} =1$.
$a_{n\space even +1} = -(-a_{n\space even}) = a_{n\space even}$ with it's first value equal to $a_{2} = -1$. So $\lim_{ n \to \infty } a_{n\space odd} =-1$. 
Because both subsequences converge to different values, $a_{n}$ diverges, even while $a_{n+1}^2$ converges.

c) Suppose that the sequence $a_n$ converges to $L$ and that, for all $n$, $a_n < 0$. Then $L < 0$.

The statement is false.
Let $a_{1} = -1$ and define $a_{n+1} = \frac{a_{n}}{2}$. 
$a_{1} = -1 < 0$, so we assume $a_{n} < 0$ for all $n$.
Consider $a_{n+1} = \frac{a_{n}}{2} < \frac{0}{2} = 0$.
So the limit of the sequence is $0$ as $n \to \infty$, but there does not exist a value $k$ such that $a_{k} = 0$.

d) If $\lim_{n \to \infty} \vert{}a_n\vert{} = 0$, then $\lim_{n \to \infty} a_n = 0$.

The statement is True.
if $\lim_{n \to \infty} \vert{}a_n\vert{} = 0$, then $\lim_{n \to \infty} a_n = \lim_{n \to \infty} \vert{} a_n \vert{}$ or $\lim_{n \to \infty} -\vert{} a_n \vert{}$. 
Because $\lim_{n \to \infty} \vert{}a_n\vert{} = 0$ and $\lim_{n \to \infty} -\vert{}a_n\vert{} = -0 =0$, $\lim_{n \to \infty} a_n = 0$.
