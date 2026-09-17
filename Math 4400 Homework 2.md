Samuel Nankervis
Math 4400, Homework 2
September 18th, 2026
Dr. Han

Questions from 1.3

1. Let $f(x) = (x + \sqrt{x})/(x^2 + 1)$.
	a) Show that $f(x) \le \begin{cases} 2\sqrt{x}, & 0 \le x \le 1 \\ 2/x, & x \ge 1 \end{cases}$
	
	If $0 \le x \le 1$, then $x \le \sqrt{x}$. So $(x+\sqrt{x})\le(\sqrt{x}+\sqrt{x}) = 2\sqrt{x}$.
	While $0 \le x \le 1$, $x^2+1 \ge 1$.
	Taking the full function into consideration, for $0 \le x \le 1$ we see that $\frac{x + \sqrt{x}}{x^2 + 1} \le \frac{2\sqrt{x}}{1} = 2\sqrt{x}$. 
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

1. Use induction to show that, for all $n \ge 1$,
	$\sum_{k=1}^{n} k^3 = \left(\sum_{k=1}^{n} k\right)^2.$
	

2. Use induction to show that
	a) $2n + 1 \le 2^n$ for $n \ge 3$.
	
	
	b) $n^2 \le 2^n + 1$ for $n \ge 1$.
	

Use PMI or generalized PMI to prove each of the following statements.

1. $\sum_{i=1}^{n} (2i - 1)^3 = n^2(2n^2 - 1).$
	
	
2. $(n + 1)! > 2^{n+3}$ for $n \ge 5$.
	
	
3. $4^n - 1$ is divisible by $3$.
	
	
4. If $a_1 = 2$, $a_{n+1} = \frac{2a_n + 4}{3}$ for $n \ge 1$, then $a_n \le 4$ for all $n$.
	
	
