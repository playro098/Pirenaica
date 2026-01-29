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

### Matrius Inverses:
La matriu és aquella que multiplicada per ella mateixa és igual a la identitat:
$$
A·A^{-1}=I
$$
Hi han matrius per les que no existeix la seva inversa, aquestes matrius s'anomenen matrius singulars.

##### Com podem saber si existeix?
Donada $A\subset M_m$,  $A^{-1} \subset$  si  $|A|$ , Es a dir, si una matriu quadrada té un $|A|$ diferent de zero aleshores té matriu inversa.
$$
A^{-1}=\frac{1}{|A|}·(A^t)^{Adj}
$$
$Adj$ = matriu adjunta
Per fer la matriu transposada adjunta elaborem una matriu de la següent manera
$$
\begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9\end{pmatrix} =\begin{pmatrix} {\begin{pmatrix} 5 & 6  \\ 8 & 9\end{pmatrix}} & {\begin{pmatrix} 4 & 6  \\ 7 & 9\end{pmatrix}} & {\begin{pmatrix} 4 & 5  \\ 7 & 8\end{pmatrix}} \\ {\begin{pmatrix} 2 & 3  \\ 8 & 9\end{pmatrix}} & {\begin{pmatrix} 1 & 3  \\ 7 & 9\end{pmatrix}} & {\begin{pmatrix} 1 & 2  \\ 7 & 8\end{pmatrix}} \\ {\begin{pmatrix} 2 & 3  \\ 5 & 6\end{pmatrix}} & {\begin{pmatrix} 1 & 3  \\ 4 & 5\end{pmatrix}} & {\begin{pmatrix} 1 & 2  \\ 4 & 5\end{pmatrix}}\end{pmatrix}
$$
Mirem la posició de cada digit en la primera matriu i ignorem la seva fila i columna, amb els quatre digits restants elaborem una matriu més petita. Per exemple en la posició 1,1:
$$
\begin{pmatrix} *1* & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9\end{pmatrix} = \begin{pmatrix} 5 & 6  \\ 8 & 9\end{pmatrix}
$$
Un cop tenim aquest monstre l'hem de simplificar de la següent manera, trobem el determinant de cadascuna d'aquestes matrius $2^2$, que és molt més fàcil ($ad-bc$) i això ens donara una matriu $3^3$ dels determinants. Ara apliquem els cofactors, és a dir canviem els signes de la següent manera:
$$
\begin{pmatrix} + & - & + \\ - & + & - \\ + & - & +\end{pmatrix}
$$
Un cop fet això podem tornar a la funció:
$$
A^{-1}=\frac{1}{|A|}·(A^t)^{Adj}
$$
I ja podem treballar amb $(A^t)^{Adj}$.
### Rang de la matriu:
Per a tota matriu de la qual les seves files són linealment dependents, les seves columnes ho seran també. 

Si bé és fàcil veure la dependencia en una matriu $2^2$, Pot ser molt més complex amb matrius més grans, la següent matriu presenta una dependencia entre les seves files d'aquesta manera:
$$
F_3=2F_1+F_2
$$
$$
\begin{pmatrix} 1 & 0 & -2 \\ 3 & 1 & 0 \\ 5 & 1 & -4\end{pmatrix}
$$
Una matriu quadrada només té inversa si el seu rang és el maxim possible, és a dir, que sigui completament relacionar les files entre sí, fins i tot si només n'hi ha una.

### Mètode de Gauss:
El rang d'una matriu esglaonada coincideix amb el nombre de files no nul·les, per exemple:
$$
\begin{pmatrix} 1 & 5 & -2 \\ 0 & 1 & 3 \\ 0 & 0 & 0\end{pmatrix} Rang=2
$$
$$
\begin{pmatrix} -2 & 4 & 3 \\ 0 & 1 & -1 \\ 0 & 0 & 2\end{pmatrix} Rang=3
$$
### Transformació de matrius:
Hi han cinc maneres de modificar les matrius sense canviar el seu rang.
1. Intercanviar de lloc dues files.
2. Multiplicar o dividir tots els elements d'una fila o columna per un nombre diferent de $0$.
3. Sumar o restar a una fila o columna els elements d'un altre línia paral·lela multiplicats per un nombre diferent de $0$.
4. Suprimir les línies les quals només contenen zeros.
5. 


### Regla de Sarrus:
Aquesta regla ens permet trobar el determinant que en dona informació sobre les característiques de la matriu. En una matriu $2^2$ el procediment és simple:
$$
\begin {pmatrix} a & b \\ c & d \end {pmatrix}
$$
$$
Det = ad-bc
$$
En una matriu $3^2$ el procediment es més complicat,
$$
\begin {pmatrix} a & b & c \\ d & e & f \\ g & h & i\end {pmatrix}
$$
$$
det=aei+bfg+cdh−ceg−bdi−afh
$$
En realitat en ambdós casos el procediment és restar les diagonals entre si, però amb matrius tres per tres , al ser intercanviables les seves files, hi ha tres diagonals per direcció. I recordem que restem sempre les diagonals de la segona direcció (esquerra a dreta) contra les de primera (dreta a esquerra).
### El determinant:
Ens dona informació en funció del seu valor
1. El determinant és nul:
	1. Té una fila o columna de zeros
	2. Té dues files o columnes iguals
	3. Té dues files o columnes proporcionals
	4. Si una fila o columna és combinació lineal d'altres
2. Si multipliquem per un nombre real tots els elements d'una fila o columna, el determinant quedara multiplicat per aquest nombre.
3. Si canviem de files o columnes el determinant el canviarem de signe.
4. Si a una fila d'un determinant li sumem una combinació lineal d'altres columnes aquest no canvia.
5. El determinant de la identitat sempre es 1
6. El determinant d'un producte de matrius quadrades és igual al producte dels seus determinant, en conseqüència, els determinants de dues matrius inverses són inversos entre sí
7. El determinant d'una matriu és identic al de la seva transposada

### Determinants de matrius de més de tres files:
Agafem una columna, acte seguit (sense comptar la columna escollida) fem tantes matrius més petites com nombre de digits tingui la fila (quatre matrius de tres per tres si trevallavem amb una de quatre per quatre). Multipliquem una d'aquestes matrius per un dels digits, repetim amb tota la resta de digits, el resultat és el determinant.

### Glossari
#### Matrius Esglaonades:


#### Matriu transposada:
Canviar files per columnes
$$
\begin{pmatrix} a & b \\ c & d \end{pmatrix} -> \begin{pmatrix} a & c \\ b & d \end{pmatrix} \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} -> \begin{pmatrix} 1 & 3 \\ 2 & 4 \end{pmatrix} 
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

Exercicis:
2021 - S5 - 1
2020 - S1 - 5
2010 - S5 - 4
2011 - S2 - 1
2012 - S1 - 5
Pagina 87
1. 30
2. 34