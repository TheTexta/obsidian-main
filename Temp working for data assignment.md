Probability of blackjack from first 2 cards through using a hypergeometric distribution. 

### Formula

$P(X) = \frac{_nC_x \cdot _{n-a}C_{r-x}}{_nC_r}$

Where
$X$ = event (ace or 10 point card)
$a$ = # of successes available  
$x$ = # of successes being chosen 
$n$ = # of objects available (52/51 Cards)
$r$ = # of objects being chosen (number of draws = 1)

### Drawing an Ace First, then a 10-Value card second
$P(\text{Ace First}) = \frac{\text{number of aces}}{\text{total number of cards}}$
$P(\text{Ace First}) = \frac{4}{52}$

$P(\text{10 Value Card Second})= \frac{_{16}C_{1}\cdot _{(51-16)}C_{(1-1)}}{_{51}C_1}$
$P(\text{10 Value Card Second}) = \frac{16\cdot 1}{51}$
$P(\text{10 Value Card Second}) = \frac{16}{51}$

$P(\text{Ace then 10 Value}) = P(\text{Ace First}) \cdot P(\text{10 Value Card Second})$
$P(\text{Ace then 10 Value}) = \frac{4}{52} \cdot \frac{16}{51}$
$P(\text{Ace then 10 Value}) = \frac{16}{663} = 2.41\%$
### Drawing an 10-Value Card, then an Ace second
$P(\text{10 Value Card First})= \frac{\text{number of 10 point cards}}{\text{total number of cards}}$
$P(\text{10 Value Card First})= \frac{16}{52}$

$P(\text{Ace Second})= \frac{_{4}C_{1}\cdot _{(51-4)}C_{(1-1)}}{_{51}C_1}$
$P(\text{Ace Second})= \frac{4\cdot 1}{51}$
$P(\text{Ace Second})= \frac{4}{51}$

$P(\text{10 Value then Ace}) = P(\text{10 Value Card First}) \cdot P(\text{Ace Second})$
$P(\text{10 Value then Ace}) = \frac{16}{52} \cdot \frac{4}{51}$
$P(\text{10 Value then Ace}) = \frac{16}{663} = 2.41\%$

### Probability of Blackjack
$P(\text{Blackjack on Draw}) = P(\text{10 Value then Ace}) + P(\text{Ace then 10 Value})$
$P(\text{Blackjack on Draw}) = \frac{16}{663} + \frac{16}{663} = \frac{32}{663} = 4.83\%$
