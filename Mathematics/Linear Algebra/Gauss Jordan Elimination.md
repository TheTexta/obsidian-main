#math133 
AKA - Gaussian Elimination

- if all entries zero stop the algorithm
- locate first nonzero leftmost column. take the row with the nonzero leftmost column and swap it for the top row and make it a one coefficient
- get rid of all subsequent numbers in the same column using that leading one
- Repeat steps 1 and 2 (ignoring top row)
- This produces a [[row echelon form|REF]]
- get [[reduced row echelon form|RREF]] by using each leading one (starting with rightmost) to get rid of all entries above