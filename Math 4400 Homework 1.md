Samuel Nankervis
September 14th, 2026
Dr. Han


Exercises for 1.1:

4. Using the fact that $1/2 > 0$, show that if $a, b \in \mathbb{R}$ with $a < b$, then $a < (a+b)/2 < b$.
	
	Using Theorem 1.2.3, we know that if $x > y$ and $z > 0$, then $xz > yz$. 
	
	We know that $a<b$. This implies that $a+a < a+b$. Because $\frac{1}{2}>0$ ,  $\frac{1}{2}(a+a)< \frac{1}{2}(a+b)$. Simplifying the inequality, we see that $a< \frac{a+b}{2}$.
	We know that $b>a$. This implies that $b+b > a+b$. Because $\frac{1}{2}>0$ ,  $\frac{1}{2}(b+b)> \frac{1}{2}(a+b)$. Simplifying the inequality, we see that $b> \frac{a+b}{2}$.
	
	Because  $a< \frac{a+b}{2}$ and $b> \frac{a+b}{2}$, then $a < \frac{a+b}{2} < b$. Thus we have shown that if $a, b \in \mathbb{R}$ with $a < b$, then $a < (a+b)/2 < b$.
	
5. a) For real numbers $a$ and $b$, show that
	$$ab \le \frac{1}{2}(a^2 + b^2).$$
	Consider $(a-b)^2$. 
	If $a-b>0$, then $(a-b)^2>0$.
	If $a-b<0$, then $(a-b)^2>0$.
	If $a-b = 0$, then $(a-b)^2 = 0$.
	
	So, $(a-b)^2\ge 0$ for all real numbers $a$ and $b$. $(a-b)^2 = a^2 + b^2 - 2ab$. So $a^2 + b^2 - 2ab\ge 0$ and $\frac{1}{2}(a^2 + b^2)\ge ab$. Thus we have proven $ab \le \frac{1}{2}(a^2 + b^2).$ 
	
	
	b) For real numbers $a, b,$ and $c$ show that
	$$ab + bc + ca \le a^2 + b^2 + c^2.$$
	From question 5a, we see that $a^2+b^2\ge 2ab$, $a^2+c^2\ge 2ac$, and $b^2+c^2\ge 2bc$. 
	So, $a^2 + b^2+a^2+c^2+b^2+c^2 \ge 2ab + 2ac + 2bc$. 
	Simplifying this inequality, we get $2(a^2+b^2+c^2) \ge 2(ab+ac+bc)$. 
	By dividing by 2 and reordering the terms, we get $ab + bc + ca \le a^2 + b^2 + c^2.$ 


7. Following the reasoning of Theorem 1.1, show that $\sqrt{3}$ is not a rational number. You may use the fact that, if 3 divides a product of integers $pq$, then it must divide either $p$ or $q$ (or perhaps both).
	
	To show that $\sqrt{ 3 }\notin \mathbb{Q}$ we show that there does not exist an $x \in \mathbb{Q}$ such that  $x^2 =3$. 
	We proceed by contradiction. 
	Suppose that there does exist an $x \in \mathbb{Q}$ such that  $x^2 =3$. Then $x = \frac{p}{q}$ with $p,q \in \mathbb{Z}$. 
	We can replace $x$ with $\frac{p}{q}$, and assume that the fraction $\frac{p}{q}$ is reduced to simplest terms. For example if $p =3\cdot2$ and $q = 3\cdot3$, then $\frac{p}{q}$ is written as $\frac{2}{3}$ instead of $\frac{6}{9}$.
	After replacing $x$ with $\frac{p}{q}$, we have $\left( \frac{p}{q} \right)^2 =3\implies \frac{p^2}{q^2} = 3$. 
	Solving for $p^2$, we see $p^2 = 3q^2$. Therefore, $p$ has a factor of $3$ and can be rewritten as $3m$ for some $m \in \mathbb{Z}$. Replacing $p^2$ with $(3m)^2$, we see that  $9m^2 = 3q^2 \implies 3m^2 = q^2$. So $q$ also has a factor of $3$, but we stated that $\frac{p}{q}$ was in simplest terms already, meaning they had no factors in common. $\Rightarrow\!\Leftarrow$
	Thus, by contradiction, there does not exist an $x \in \mathbb{Q}$ such that  $x^2 =3$, and we have shown that $\sqrt{ 3 }\notin \mathbb{Q}$.
	

Exercises for 1.2:

5. Find the sup and inf of the following sets when they exist as finite numbers. If either a sup or an inf is not finite, explain why.
    
	a) $A = \{1 + (-1)^n(n-1)/n : n \in \mathbb{N}\}$.
	To illustrate the patterns in the sequence, I will list the first few values of it. ${1-0, 1+\frac{1}{2},1-\frac{2}{3},1+\frac{3}{4}\dots}$
	The fractional portion of the series approaches $1$ as $n \to \infty$. We can find this by taking the limit of $\frac{n-1}{n}$ as $n \to \infty$. The $(-1)^n$ factor will alternate between positive and negative for even and odd values. For even values of $n$ approaching $\infty$, the series approaches $1+1=2$. For odd values of $n$ approaching $\infty$, the series approaches $1-1=0$. Thus the infimum of the series is $0$ and the supremum is $2$.
	
	b) $B = \{x \in \mathbb{Q} : x^3 < 5x\}$.
	First to find the supremum, we can simplify the set $B$ by rewriting the condition as $B = \{x \in \mathbb{Q} : x^2 < 5\}$. This is not true for values of $x < 0$, but the set has positive values that are greater than all of the negative values in the set, so the supremum will be positive. We know from Theorem 1.1 that for all $x \in \mathbb{Q}$, there does not exist an $x$ such that $x^2 = 5$, since $5$ is not a perfect square. So $\sqrt{ 5 }$ is an upper bound for the set. Consider the real number $M\in\mathbb{R}$ such that $M\le\sqrt{5}$ . 
	If $M\le \sqrt{5}$, then all values of $x\in B$ are greater than $M$. If $-\sqrt{5} < M < \sqrt{5}$, we apply the density of rational numbers in $\mathbb{R}$, which states that between any two distinct real numbers, there exists a rational number $q \in \mathbb{Q}$.Considering the open interval $(M, \sqrt{5})$, density guarantees a rational number $q$ such that $M < q < \sqrt{5}$. Because $-\sqrt{5} < M < q < \sqrt{5}$, we have $q^2 < 5$ and $q \in \mathbb{Q}$, which means $q \in B$. Since $q \in B$ and $q > M$, $M$ cannot be an upper bound for $B$.
	We can see that $\sqrt{ 5 }$ is the least upper bound for the set $B$, or the supremum of $B$.  
	
	There is no finite infimum for the set, because the Greatest Lower Bound Property requires the set to be bounded from below. As $x\to-\infty$, $x^3\to-\infty$ at a faster rate than $5x\to-\infty$. This can be confirmed by taking the limit as $x\to-\infty$ of $\left( \frac{x^3}{5x} \right)$. 

###### **Problem 1.** Find the sup and inf of the following sets when they exist as finite numbers.

Notations: $\mathbb{N} = \{1, 2, 3, \dots\}$. $\mathbb{Z} = \{\dots, -1, 0, 1, 2, 3, \dots\}$.

$\mathbb{Q} = \{\frac{m}{n} : m, n \in \mathbb{Z}, n \neq 0\}$. $\mathbb{R} = (-\infty, \infty)$.

a) $A = \{-1, \frac{1}{2}, -\frac{1}{3}, \dots, \frac{(-1)^n}{n}, \dots\}$.
To find the supremum and infimum, we can break the set into two different categories for if $n$ even or odd. So $A_{even} = {\frac{1}{2n}}$ and $A_{odd} = {\frac{-1}{2n}}$. Both of the sets approach $0$ as $n\to\infty$. So the first values are more extreme than any others in the set. Thus, the infimum is $-1$, the first odd, negative value, and the supremum is $\frac{1}{2}$, the first even, positive value.

b) $B = \{x \in \mathbb{Q} : x^2 < 7\}$.
We can find the infimum and supremum similarly to how I answered 5b. We know from Theorem 1.1 that for all $x \in \mathbb{Q}$, there does not exist an $x$ such that $x^2 = 7$, since $7$ is not a perfect square. So $\sqrt{ 7 }$ is an upper bound for the set. Consider the real number $M\in\mathbb{R}$ such that $M\le\sqrt{7}$ . 
If $M\le -\sqrt{7}$, then all values of $x\in B$ are greater than $M$. 
If $-\sqrt{7} < M < \sqrt{7}$, we apply the density of rational numbers in $\mathbb{R}$, which states that between any two distinct real numbers, there exists a rational number $q \in \mathbb{Q}$. Considering the open interval $(M, \sqrt{7})$, density guarantees a rational number $q$ such that $M < q < \sqrt{7}$. Because $-\sqrt{7} < M < q < \sqrt{7}$, we have $q^2 < 7$ and $q \in \mathbb{Q}$, which means $q \in B$. Since $q \in B$ and $q > M$, $M$ cannot be an upper bound for $B$.
We can see that $\sqrt{ 7 }$ is the least upper bound for the set $B$, or the supremum of $B$.  

We also know that $-\sqrt{ 7 }$ is also a lower bound for $B$ using the same Theorem 1.1 as above. Consider the real number $M\in\mathbb{R}$ such that $M\ge-\sqrt{7}$ . 
If $M\ge \sqrt{7}$, then all values of $x\in B$ are less than $M$. 
If $-\sqrt{7} < M < \sqrt{7}$, we apply the density of rational numbers in $\mathbb{R}$, which states that between any two distinct real numbers, there exists a rational number $q \in \mathbb{Q}$. Considering the open interval $(-\sqrt{7},M)$, density guarantees a rational number $q$ such that $-\sqrt{7} < q < M$. Because $-\sqrt{7} < q < M < \sqrt{7}$, we have $q^2 < 7$ and $q \in \mathbb{Q}$, which means $q \in B$. Since $q \in B$ and $q < M$, $M$ cannot be a lower bound for $B$. So $-\sqrt{ 7 }$ is the infimum of $B$.

c) $C = \{x \in \mathbb{N} : x^2 > 7\}$.

$C$ does not have a supremum, because $x^2\to\infty$ while 7 remains constant. So $C$ is not bounded from above. 

$3$ is the infimum of the set $C$. $3^2 = 9$, so $3^2>7$, and $3$ is a lower bound of $C$. The next lowest natural number is $2$. $2^2 = 4$, so $2^2 < 7$. All other Natural numbers less than $2$ will have squared values less than $2^2$. So $3$ is the infimum of the set $C$.

d) $D = \{x \in \mathbb{Z} : x^2 < 111\}$.

We can solve d) similarly to how we solved c). Consider $x=10$. $x^2 = 100$, so $x^2<111$. The next largest integer is $11$. If $x=11$, $x^2 = 121$, and $x^2>111$. So $10$ is an upper bound for $D$ while $11$ is not, and thus $10$ is the least upper bound or supremum of $D$.

Consider $x=-10$. $x^2 = 100$, so $x^2<111$. The next smallest integer is $-11$. If $x=-11$, $x^2 = 121$, and $x^2>111$. So $-10$ is a lower bound for $D$ while $-11$ is not, and thus -$10$ is the greatest lower bound or infimum of $D$.

###### **Problem 2.** Prove that there does not exist a rational number $x$ such that $x^2 = 125$.

To prove that there does not exist a rational number $x$ such that $x^2 = 125$, we proceed by contradiction. Suppose that there does exist a rational number $x$ such that $x^2 = 125$. Since $x \in \mathbb{Q}$ , $x = \frac{p}{q}$ for some $p \in \mathbb{Z}$ and $q \in \mathbb{Z}$  with $q \neq 0$. 

So, $x^2 = 125 \implies (\frac{p}{q})^2 = 125\implies \frac{p^2}{q^2} = 5^3$ . Multiplying both sides by $q^2$ gives $p^2 = 5^3q^2$ . 

Since $p$ and $q$ are squared, we know that the prime factorization of $p^2$ and $q^2$ will contain an even number of 5's as prime factors. However, $5^3$ has an odd number of factors of 5's and $q^2$ has an even number of factors of 5's. Since the powers of 5's will add together when multiplied, $q^2 5^3$ has an odd number of factors of 5's. But $p^2$ has an even number of factors of 5's, and $p^2 = q^25^3$ . $\Rightarrow\!\Leftarrow$

Thus, we have found a contradiction. Therefore, there is no rational solution for $x^2 = 125$.
