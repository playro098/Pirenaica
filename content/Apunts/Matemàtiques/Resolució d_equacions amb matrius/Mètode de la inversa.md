Posem per cas que tenim el següent sistema:
$$
\begin{cases} x-y+3z=0 \\ 2x-2y+z=1 \\ y-z=-1 \end{cases} 
$$
Aquest cop escriurem dues matrius: $A$ com abans I $B$ només incloent els termes independents:
$$
A=\begin{pmatrix} 1&-1&3\\2&-2&1\\0&1&-1 \end{pmatrix} \qquad B= \begin{pmatrix} 0\\1\\-1 \end{pmatrix}
$$
Podem fer la següent deducció:
$$
A·X=B \Rightarrow B·A^{-1}=X
$$
Nosaltres tenim $A$ i $B$, si $A$ és invertible també tenim $A^{-1}$ 