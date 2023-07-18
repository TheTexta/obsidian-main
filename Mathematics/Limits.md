A limit is the value of a function as it approaches a certain point. For a limit to exist it has to be [[Real Limits|real]] and not [[Infinite Limits|infinite]]. Which is checked through the comparison of the left/right hand of the limit. Limits require do not require [[Continuity]].

## Basic Definition
$L = \lim_{x \to c} f(x)$
Where L is the value f(x) approaches as the x value gets closer to c.

### Left Hand v Right Hand
Limits have a left and right hand side, which describes the value the function approaches when the x value gets closer on the left hand side vs the right.

#### Left
$L = \lim_{x\to c^-}f(x)$
#### Right
$L = \lim_{x\to c^+}f(x)$

## Limit Theorems
###### Constant Rule
$\lim_{x\to c}(k) = k$
###### Constant multiple rule
$\lim_{x \to c}(k \cdot f(x))=k \cdot \lim_{x \to c}f(x)$
###### Sum Rule
$\lim_{x\to c}(f(x)+g(x))=\lim_{x\to c}f(x) + \lim_{x\to c}g(x)$
###### Product Rule
$\lim_{x\to c}(f(x)\cdot g(x))=\lim_{x\to c}f(x) \cdot \lim_{x\to c}g(x)$
###### Composition Rule
$\lim_{x \to c}f(g(x)) = f(\lim_{x\to c}g(x))$
###### Sandwich Square Theorem
$\text{if } f(x)\leq g(x)\leq h(x) \text{ and } \lim_{x\to c}h(x) = \lim_{x\to c}f(x)=L \text{ than the } \lim_{x \to c}g(x) = L$
###### Big Number Theorem :)
$\lim_{x\to \infty}\frac{1}{x}=0$

## Limits of $\infty$ for rational functions
$\lim_{x\to c}\frac{P(x)}{Q(x)}$ 
* if P's degree is less then Q's then the limit equals 0
* If P's degree is equal to Q's then the limit equals the leading coefficient of P over the leading coefficient of Q
* If P's degree is greater then Q's then the limit equals $\pm \infty$.

## Limits of Trigonometric Functions
$lim_{x\to 0}\frac{sinx}{x}=1$
$lim_{x\to 0}\frac{1-cosx}{x}=0$

## Proving Trig Function Limits
$lim_{x\to \infty}\frac{sinx}{x}=0$ because for all values of $sinx$ it is $-1\leq sinx \leq 1$ so it follows that $-\frac{1}{x} \leq \frac{sinx}{x} \leq \frac{1}{x}$and because $lim_{x\to\infty}\pm\frac{1}{x}=0$ factor squeeze theorem shows that $lim_{x\to\infty}\frac{sinx}{x} = 0$.