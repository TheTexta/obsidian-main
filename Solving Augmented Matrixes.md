#math133 
Through [[Elementary Operations]] and [[Elementary Row Operations]] we can solve [[Augmented Matrix|augmented matrices]] by operating on them to reach a [[Row Echelon Form]] like below, where the astrarix represents an arbitrary number.
$$\begin{pmatrix}  
1 & 0 & 0& |*\\  
0 & 1 & 0&|*\\
0 & 0 & 1&|*\\
\end{pmatrix}$$

## Steps
1. Start with the leftmost column (known as the pivot column)
2. Identify the pivot row (row with the highest [[Absolute Function|absolute value]]) and place it at the top row
3. Divide the pivot row by itself to normalise its coefficient to one
4. Use [[Elementary Row Operations]] to eliminate the coefficients of all the other rows
5. Move to the next column and repeat