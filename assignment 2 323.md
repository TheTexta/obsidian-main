Q1.
$$
P(GS\,|\,\text{silver})=\frac{P(\text{silver}\,|\,GS)P(GS)}{P(\text{silver}\,|\,SS)P(SS)+P(\text{silver}\,|\,GS)P(GS)}=\frac{(1/2)(1/3)}{(1)(1/3)+(1/2)(1/3)}=\frac{1/6}{1/2}=\frac{1}{3}.

$$

The other box is gold exactly when the drawer is $GS$, so the required probability is $\frac{1}{3}$​.





Q2.
$$ \text{Total ways}=\binom{8}{4}=70, \quad \text{favorable}=\binom{3}{2}\binom{5}{2}=3\cdot10=30$$
$$P(\text{exactly 2 undergrads})=\frac{\binom{3}{2}\binom{5}{2}}{\binom{8}{4}}
=\frac{30}{70}=\frac{3}{7}$$





Q3.
$$\text{Total ways} = \binom{10}{5} = 252,
\quad
\text{Favorable ways} = \binom{6}{5} = 6,$$

$$P(\text{all 5 solvable}) = \frac{\binom{6}{5}}{\binom{10}{5}}
= \frac{6}{252}
= \frac{1}{42}$$





Q4.
Let $R_i$ be the event “relay $i$ closes,” with $Pr(R_i)=0.9$ and independence.
	a)
		Current flows iff **at least one** of the three relays closes:
		
		$\Pr(\text{flow}) = 1 - \Pr(\overline{R_1} \cap \overline{R_2} \cap \overline{R_3}) = 1 - (0.1)^3 = 0.999$
	b)
		We want $Pr(R_1|flow)$. since $R_1 \subseteq$ flow,
		$\Pr(R_1 \mid \text{flow}) = \frac{\Pr(R_1)}{\Pr(\text{flow})} = \frac{0.9}{0.999} = \frac{100}{111} \approx 0.9009$





Q5.
The probability that a defective item gets by both inspectors is found by multiplying
the probability it passes the first inspector by the probability it also passes the second
given it passed the first. 

$P(\text{pass 1st}) = 0.1$
$P(\text{pass 2nd} \mid \text{pass 1st}) = 0.5$
$P(\text{pass both}) = 0.1 \times 0.5 = 0.05$







Q6.
Given:
$P(I) = 0.10, \quad P(II) = 0.15, \quad P(I \cap II) = 0.03$

a)
	Probability of at least one disease:
	$P(I \cup II) = P(I) + P(II) - P(I \cap II)$
	$= 0.10 + 0.15 - 0.03 = 0.22$
	
	$P(\text{at least one disease}=0.22$

b)
	Conditional probability of both diseases given at least one:
	$P(I \cap II \mid I \cup II) = \frac{P(I \cap II)}{P(I \cup II)}$
	$= \frac{0.03}{0.22}$

	$P(\text{both} \mid \text{at least one}=\frac{3}{22}\approx 0.136363636$








Q7.
Time Budget: If the $k$-th typed donor is the first match, total time is $2k + 2$ minutes. We need $2k+2 \le 10 \implies k \le 4$. So we can type at most $4$ donors and still complete the transfusion in time.

Success event: At least one of the first $4$ donors is A$^+$.
$P(\text{saved}) \;=\; 1 - (1-p)^4 \;=\; 1 - 0.6^4= 1 - 0.1296 = 0.8704$

$P(\text{victim saved})=0.8704$








Q8.
a)
	$\text{“Last defective on the 4th test”} \iff \text{one defective is at position }4\text{ and the other is in }\{1,2,3\}.$
	$P = \dfrac{\binom{1}{1}\cdot 3}{\binom{6}{2}} = \dfrac{3}{15} = \tfrac{1}{5}$

b)
	$\text{Both defectives found by the 4th test} \iff \text{both defectives are among the first 4 positions}.$
	$P = \dfrac{\binom{4}{2}}{\binom{6}{2}} = \dfrac{6}{15} = \tfrac{2}{5}$

c)
	Given exactly one defective in the first two tests.
	Remaining 4 items have 1 defective and 3 good. We want a defective in tests 3 or 4.
	$P = 1 - P(\text{both next two are good}) = 1 - \left(\frac{3}{4}\cdot\frac{2}{3}\right) = 1 - \frac{1}{2} = \tfrac{1}{2}$








Q9.
By Bayes’ theorem:
$$P(A|F) = \frac{P(F|A)P(A)}{P(F|A)P(A) + P(F|B)P(B)}$$
$$= \frac{(0.2)(0.7)}{(0.2)(0.7) + (0.1)(0.3)}$$
$$= \frac{0.14}{0.14 + 0.03} = \frac{0.14}{0.17} = 0.8235$$
$$P(A|F) = 0.8235$$







Q10.
a)
	$P(A)=P(A\mid B)P(B)+P(A\mid \overline B)P(\overline B) =pP(B)+p(1-P(B))=p$
	Hence:
	$P(A\cap B)=P(A\mid B)P(B)=p\,P(B)=P(A)P(B)$, so $A$ and $B$ are independent.

b)
	$P(A)=P(A\mid C)P(C)+P(A\mid \overline C)\,P(\overline C)$, $P(B)=P(B\mid C)P(C)+P(B\mid \overline C)\,P(\overline C).$
	Subtract to get
	$P(A)-P(B)=\big(P(A\mid C)-P(B\mid C)\big)P(C)+\big(P(A\mid \overline C)-P(B\mid \overline C)\big)P(\overline C)$
	Given $P(A\mid C)>P(B\mid C)$ and $P(A\mid \overline C)>P(B\mid \overline C)$, each bracket is positive, and $P(C),P(\overline C)>0$, so the RHS $>0$. Therefore $P(A)>P(B)$.