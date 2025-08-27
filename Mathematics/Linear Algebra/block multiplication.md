#math133 
$A=\left(\begin{array}{cc:ccc}1 & 0 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 & 0 \\ \hdashline 2 & 3 & 1 & 2 & 1 \\ 1 & -1 & 3 & 0 & 2\end{array}\right)=\pmatrix{I_2&O_{2\times 3}\\P_{2\times 2}&Q_{2\times 3}}$ 
$B=\left(\begin{array}{cc}1 & -1 \\ 0 & 1 \\ 2 & 1 \\ 3 & 1 \\ 1 & -1\end{array}\right)=\pmatrix {R_{2\times 2}\\S_{3\times 2}}$ 

Then $AB$ can be computed as if the blocks were single entries.
$$AB=\pmatrix{I_2&O_{2\times 3}\\P_{2\times 2}&Q_{2\times 3}}\pmatrix {R_{2\times 2}\\S_{3\times 2}}$$
$$=\pmatrix{{I_2 R_{2 \times 2}+O_{2 \times 3} S_{3 \times 2}}\\{P_{2 \times 2} R_{2 \times 2}+Q_{2 \times 3} S_{3 \times 2}}}$$
$$=\pmatrix{R+0_{2\times 2}\\PR+QS}$$
$$=\pmatrix{R\\PR+QS}$$
