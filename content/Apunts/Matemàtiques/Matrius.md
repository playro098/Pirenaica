Una matriu és un quadre de nombre de files i columnes $m·n$ 
Hi han matrius $m$, és a dir, quadrades, per exemple:
$$
\begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}=A_m
$$
### Suma i resta de matrius:
Tant la suma com la resta són extremadament simples, l'únic que cal fer és restar cada terme pel seu equivalent en l'altre matriu. Les matrius han de tenir les mateixes dimensions per fer possible la suma o resta:
$$
A = \begin{bmatrix} 2 & 5 \\ 1 & 3 \end{bmatrix}, \quad
B = \begin{bmatrix} 4 & 1 \\ 7 & 2 \end{bmatrix}
$$
$$
A + B = \begin{bmatrix} 2+4 & 5+1 \\ 1+7 & 3+2 \end{bmatrix} = \begin{bmatrix} 6 & 6 \\ 8 & 5 \end{bmatrix}
$$
### Multiplicació de matrius:
Per multiplicar dues matrius multipliquem columna per fila. Per exemple, si volem trobar el nombre que quedarà en la posició 1,1 multiplicarem el primer nombre de la primera fila de la primera matriu pel nombre de la primera columna de la segona, pel nombre en posició i hi sumarem el segon nombre de la primera columna multiplicat pel segon nombre de la primera fila. Per exemple suposem dues matrius $2^2$

$$
A = \begin{bmatrix}1 & 2\\3 & 4\end{bmatrix}, \quad 
B = \begin{bmatrix}5 & 6\\7 & 8\end{bmatrix}
$$
Multipliquem $AB$: 
$$
AB = \begin{bmatrix}
1\cdot5 + 2\cdot7 & 1\cdot6 + 2\cdot8\\
3\cdot5 + 4\cdot7 & 3\cdot6 + 4\cdot8
\end{bmatrix} =
\begin{bmatrix}19 & 22\\43 & 50\end{bmatrix}
$$
Cal ressaltar que les matrius (per norma general) no són commutatives, donat com es multipliquen. Podem aprofitar l'exemple anterior per comprovar-ho:
Multipliquem $BA$:
$$
BA = \begin{bmatrix}
5\cdot1 + 6\cdot3 & 5\cdot2 + 6\cdot4\\
7\cdot1 + 8\cdot3 & 7\cdot2 + 8\cdot4
\end{bmatrix} =
\begin{bmatrix}23 & 34\\31 & 46\end{bmatrix}
$$
$$
AB \neq BA
$$
Cal ressaltar que les matrius (per norma general) no són commutatives, donat com es multipliquen. En el cas que si que ho fossin serien matrius **ortogonals**.

##### Propietats de les matrius:
Si bé no són commutatives, les matrius són **associatives** i **distributives**:
Associativa: $ABC=A(BC)=(AB)C$
Distributiva: $A(B+C)=AB+AC$ 

### Potencies de matrius:
Només es poden realitzar amb matrius quadrades. Hi han dos tipus de matrius notables en torn al resultat de multiplicar-les per elles mateixes:
- #### Idempotents:  
    - Sempre donen el mateix, es a dir: $A=A^2=A^3=A^n$ 
- #### Cícliques:
    - Al repetir la potencia un cop i un altre tornem a l'inici, per exemple: 
      $A^2=B$, $B·A= A^3 =C$, $C·A=A^4=A$ 
    - Aquesta es repetiria cada cop que l'elevem quatre vegades.
També ens poden demanar que trobem la relació cada cop que les multipliquem, per exemple
$$
\begin{pmatrix} 2 & 0 \\ 0 & 2 \end{pmatrix}^2 = \begin{pmatrix} 4 & 0 \\ 0 & 4 \end{pmatrix}
$$
En aquest cas la matriu és podria expressar així quan veiem que cada multiplicació multiplica per dos els nombres en posicions $1,1$ i $2,2$: (amb $n$ com nombre de cops que elevem la matriu)
$$
\begin{pmatrix} 2^n & 0 \\ 0 & 2^n \end{pmatrix}
$$
### Equacions Matricials:
Una equació matricial és una equació on les incògnites i/o les variables apareixen en forma de matrius en lloc de nombres reals o complexos. Com podria ser:
$$
A=BX
$$
O en formes més complexes:
$$
AX+XB=C
$$
$$
X^2+AX+B=0
$$
#### Factor comú:
Si volem treure factor comú cal tenir en compte la no commutabilitat de les matrius. No el podrem treure si no està al mateix lloc en totes les equacions. Per exemple, suposem que tenim l'equació matricial:

$$
X^2 + AX + BX + C X + DXB + EX^2 = 0
$$

On $X$ és la matriu desconeguda i $A,B,C,D,E$ són matrius conegudes de la mateixa mida que $X$.
Termes que multipliquen $X$ a la dreta: $AX, BX, CX,X^2,EX^2$  

$$
AX + BX + CX + EX^2+X^2 = (A + B + C+X(E+I)) X
$$

Termes com $DXB$  no es poden factoritzar ni a l’esquerra ni a la dreta, només reagrupar amb associativitat, que en aquest cas no ens serveix de res.

$$
DXB = D (X B) = (DX) B
$$

Per tant l'equació ens quedarà:

$$
DXB+(A + B + C+X(E+I)) X=0
$$



### Glossari
#### Matriu transposada:
Canviar files per columnes
$$
\begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} -> \begin{pmatrix} 1 & 3 \\ 2 & 4 \end{pmatrix}
$$
#### Matrius commutatives:
$A·B=B·A$
#### Inversa:
$A·A^-1=I$ 
No es pot fer quan A és proporcional, amb files buides o idèntiques
#### Idempotent
$A=A^2=A^3=A^n$
#### Ortogonal:
$A·A^t=I$

