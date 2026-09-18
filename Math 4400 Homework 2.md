Samuel Nankervis
September 18th, 2026
Math 4400, Homework 2
Dr. Han

Questions from 1.3

1. Let $f(x) = (x + \sqrt{x})/(x^2 + 1)$.
	a) Show that $f(x) \le \begin{cases} 2\sqrt{x}, & 0 \le x \le 1 \\ 2/x, & x \ge 1 \end{cases}$
	
	If $0 \le x \le 1$, then $x \le \sqrt{x}$. So $(x+\sqrt{x})\le(\sqrt{x}+\sqrt{x}) = 2\sqrt{x}$.
	While $0 \le x \le 1$, $x^2+1 \ge 1$.
	Taking the full function into consideration, for $0 \le x \le 1$, we see that $\frac{x + \sqrt{x}}{x^2 + 1} \le \frac{2\sqrt{x}}{1} = 2\sqrt{x}$. 
	If $x\ge 1$, then $x \ge \sqrt{x}$. So $(x+\sqrt{x})\le(x+x) = 2x$.
	While $x \ge 1$, $x^2+1 \ge x^2$.
	Taking the full function into consideration, for $x \ge 1$ we see that $\frac{x + \sqrt{x}}{x^2 + 1} \le \frac{2x}{x^2} = \frac{2}{x}$. 
	Therefore, for all cases of the piecewise function, $f(x) \le \begin{cases} 2\sqrt{x}, & 0 \le x \le 1 \\ 2/x, & x \ge 1 \end{cases}$
	
	b) Make similar lower estimates for $f$ on $x \ge 1$ and on $0 \le x \le 1$.
	If $0 \le x \le 1$, then $x \le \sqrt{x}$. So $(x+\sqrt{x})\ge(x+x) = 2x$.
	While $0 \le x \le 1$, $x^2+1 \le 2$.
	Taking the full function into consideration, for $0 \le x \le 1$ we see that $\frac{x + \sqrt{x}}{x^2 + 1} \ge \frac{2x}{2} = x$.
	If $x\ge 1$, then $x \ge \sqrt{x}$. So $(x+\sqrt{x})\ge(\sqrt{x}+\sqrt{x}) = 2\sqrt{x}$.
	While $x \ge 1$, $x^2+1 \le 2x^2$.
	Taking the full function into consideration, for $x \ge 1$ we see that $\frac{x + \sqrt{x}}{x^2 + 1} \ge \frac{2\sqrt{ x }}{2x^2} = \frac{\sqrt{x}}{x^2}$. 
	Therefore, for all cases of the piecewise function, $f(x) \ge \begin{cases} x, & 0 \le x \le 1 \\ \sqrt{x}/x^2, & x \ge 1 \end{cases}$ 

Questions from 1.4

2. Use induction to show that, for all $n \ge 1$,
	$\sum_{k=1}^{n} k^3 = \left(\sum_{k=1}^{n} k\right)^2$.
	
	First, we consider the lowest value of $n$. For $n=1$, the left hand side is $\sum_{k=1}^{1}k^3 = 1^3 = 1$. 
	The right hand side in this case is $(\sum_{k=1}^{1}k)^2 = 1^2 = 1$. So the statement is true for $n=1$.
	We can now assume that the statement is true for $n$.
	(1)	$\sum_{k=1}^{n} k^3 = \left(\sum_{k=1}^{n} k\right)^2$.
	Consider $n+1$,
	$\left(\sum_{k=1}^{n+1} k\right)^2 = \left(\sum_{k=1}^{n} k + (n+1)\right)^2 =$
	(2)	$\left(\sum_{k=1}^{n} k\right)^2 + 2\cdot (n+1)\cdot \left(\sum_{k=1}^{n} k\right)+(n+1)^2$.
	We can substitute the equation for $\left(\sum_{k=1}^{n} k\right)^2$  from (1) into (2).
	$\sum_{k=1}^{n} k^3 + 2\cdot(n+1)\cdot \left(\sum_{k=1}^{n} k\right)+(n+1)^2$.
	
	Now we consider the left hand side for $n+1$, $\sum_{k=1}^{n+1} k^3 = (\sum_{k=1}^{n} k^3)+(n+1)^3$.
	If $(n+1)^3 = 2\cdot(n+1)\cdot \left(\sum_{k=1}^{n} k\right)+(n+1)^2$, then $\sum_{k=1}^{n+1} k^3 = \left(\sum_{k=1}^{n+1} k\right)^2$.
	We know that $\left(\sum_{k=1}^{n} k\right) = \frac{n(n+1)}{2}$. Substituting this into the equation above, we see that
	$2\cdot(n+1)\cdot \frac{n(n+1)}{2}+(n+1)^2 = n\cdot(n+1)^2+(n+1)^2=n^3+3n^2+3n+1=(n+1)^3$.
	Because $(n+1)^3 = 2\cdot(n+1)\cdot \left(\sum_{k=1}^{n} k\right)+(n+1)^2$, we know that $\sum_{k=1}^{n+1} k^3 = \left(\sum_{k=1}^{n+1} k\right)^2$. 
	By the principle of mathematical induction, the statement is true for all $n$, because the statement is true for the lowest case of $n$ and is always true for $n+1$.

4. Use induction to show that
	a) $2n + 1 \le 2^n$ for $n \ge 3$.
	First, we consider the lowest value of $n$. For $n=3$, the right hand side is $2^3 = 8$. The left hand side is $2\cdot3+1 = 7$. So the statement is true for $n=3$.
	We can now assume that the statement is true for $n$.
	So $2n + 1 \le 2^n$ for $n \ge 3$.
	Let's consider $n+1$. 
	$2^{n+1}= 2^n\cdot (n+1)$. Substituting $2^n$ for $2n+1$, we see that $2^n\cdot (n+1)\ge (2n+1)\cdot (n+1) =2n^2+3n+1$. 
	Considering the left hand side of the equation for $n+1$, we see that $2\cdot (n+1)+1 = 2n+3$ .
	For $n\ge 3$, $2n^2 \ge 2n$, $3n \ge 3$ and $1 \ge 0$. So $2n^2+3n+1 \ge 2n+3$. Since we have shown that $2^{n+1} \ge 2\cdot (n+1)+1$, by the principle of mathematical induction, the statement is true for all $n$, because the statement is true for the lowest case of $n$ and is always true for $n+1$.
	
	b) $n^2 \le 2^n + 1$ for $n \ge 1$.
	First, we consider the lowest value of $n$. For $n=1$, the right hand side is $2^1+1 = 3$. The left hand side is $1^2 = 1$. So the statement is true for the lowest possible $n$.
	We can now assume that the statement is true for $n$.
	So $n^2 \le 2^n + 1$ for $n \ge 1$.
	Let's consider $n+1$. 
	The right hand side is: $2^{n+1}=2^n\cdot 2$.
	The left hand side is: $(n+1)^2=n^2+2n + 1$.
	For $n\ge 4$, $2^n\ge n^2\ge 2n+1$. So while $n\ge 4$, $2^n\cdot 2 \ge n^2+2n+1$. Thus, by the principle of mathematical induction, the statement is proven for all $n \ge 4$. To prove the statement for $2$ and $3$, we can simply test each value.
	For $n=2$, the right hand side is $2^2+1 = 5$. The left hand side is $2^2 = 4$.
	For $n=3$, the right hand side is $2^3+1 = 9$. The left hand side is $3^2 = 9$.
	With values for $1$, $2$, and $3$ proven, we have shown that $n^2 \le 2^n + 1$ for $n \ge 1$.

Use PMI or generalized PMI to prove each of the following statements.

1. $\sum_{i=1}^{n} (2i - 1)^3 = n^2(2n^2 - 1)$.
	First, we consider the lowest value of $n$. For $n=1$, the right hand side is $1^2(2\cdot 1^2-1) = 1$. The left hand side is $(2\cdot 1-1)^3 = 1$. So the statement is true for the lowest possible $n$.
	We can now assume that the statement is true for $n$.
	So $\sum_{i=1}^{n} (2i - 1)^3 = n^2(2n^2 - 1)$.
	Consider $n+1$ for the left hand side, $\sum_{i=1}^{n+1} (2i - 1)^3 =(\sum_{i=1}^{n} (2i - 1)^3)+(2\cdot(n+1)-1)^3$.
	We can substitute $\sum_{i=1}^{n} (2i - 1)^3$ for $n^2(2n^2 - 1)$ on the left hand side. 
	This yields $n^2(2n^2 - 1)+(2\cdot(n+1)-1)^3 = 2n^4+8n^3+11n^2+6n+1$.
	Consider $n+1$ for the right hand side, $(n+1)^2(2(n+1)^2 - 1) = (n^2+2n+1)\cdot(2n^2+4n+1) = 2n^4+8n^3+11n^2+6n+1$.
	Since we have shown that $\sum_{i=1}^{n} (2i - 1)^3 = n^2(2n^2 - 1)$, by the principle of mathematical induction, the statement is true for all $n$, because the statement is true for the lowest case of $n$ and is always true for $n+1$.
	
2. $(n + 1)! > 2^{n+3}$ for $n \ge 5$.
	
	First, we consider the lowest value of $n$. For $n=5$, the right hand side is $2^{5+3} = 256$. The left hand side is $(5+1)! = 6! = 720$. So the statement is true for the lowest possible $n$.
	We can now assume that the statement is true for $n$.
	So $(n + 1)! > 2^{n+3}$ for $n \ge 5$.
	Consider $n+1$ for the left hand side, $((n+1)+1)! = (n+2)! = (n+1)! \cdot (n+2) > 2^{n+3}\cdot (n+2)$. 
	Consider $n+1$ for the right hand side, 
	$2^{(n+1)+3} = 2^{n+4} = 2^{n+3}\cdot 2$.
	Because $n \ge 5$, $(n+2)\ge 2$. So $2^{n+3}\cdot (n+2) > 2^{n+3}\cdot 2$.
	Since we have shown that $(n + 1)! > 2^{n+3}$ for $n \ge 5$, by the principle of mathematical induction, the statement is true for all $n$, because the statement is true for the lowest case of $n$ and is always true for $n+1$.
	
3. $4^n - 1$ is divisible by $3$.
	
	First, we can rewrite the statement into an equation. 
	There exists some $a\in \mathbb{Z}$ such that $4^n-1 = 3\cdot a$.
	Next, we consider the lowest value of $n$. For $n=1$, the left hand side is $4^1-1 = 3$. $3\cdot 1 = 3$, so $a=1$ when $n=1$, and the statement is true for the lowest possible $n$.
	We can now assume that the statement is true for $n$.
	So there exists some $a\in \mathbb{Z}$ such that $4^n-1 = 3\cdot a$.
	Now we consider $n+1$. $4^{n+1}-1=4\cdot 4^n -1$.
	We know that $4^n=3a+1$. Substituting this into our previous step, we see that $4\cdot 4^n -1 = 4\cdot (3a +1) -1 = 12a+3$. $12$ has factors $4$ and $3$, so we can combine $a$ with $4$ while still keeping $a\in \mathbb{Z}$ to get $3a+3$. Additionally, we see that $3a+3 = 3(a+1)$, and $a+1 \in \mathbb{Z}$. So we have $3\cdot a$.
	Since we have shown that $4^n - 1$ is divisible by $3$, by the principle of mathematical induction, the statement is true for all $n$, because the statement is true for the lowest case of $n$ and is always true for $n+1$.
	
4. If $a_1 = 2$, $a_{n+1} = \frac{2a_n + 4}{3}$ for $n \ge 1$, then $a_n \le 4$ for all $n$.
	
	First, we consider the lowest value of $n$. For $n=1$, $a_{1} =2 \le 4$.
	We can now assume that the statement is true for $n$.
	So $a_n\le 4$.
	Consider $a_{n+1}$, 
	$a_{n+1} = \frac{2a_n + 4}{3}$. Because $a_n\le 4$, $\frac{2a_n + 4}{3} \le \frac{2(4) + 4}{3} =4$.
	Thus, $a_{n+1} \le 4$. By the principle of mathematical induction, the statement is true for all $n$, because the statement is true for the lowest case of $n$ and is always true for $n+1$.
	