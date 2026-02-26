Aquest és normalment el mètode més simple i el primer que cal fer és convertir la matriu en esglaonada com ja faríem normalment.
$$
\left(
\begin{array}{ccc|c}
1 & -1 & 1 & 0 \\
-3 & 2 &  0 & 1 \\
-5 & 2 &  4 & 12
\end{array}
\right) \Rightarrow \left( \begin{array}{ccc|c}
1 & -1 &1&0 \\ 0&-1&3&10 \\ 0&0&0&18
\end{array} \right)
$$
A partir d'aquí hem de comprovar varies coses: (recordem, matriu $A$ és sense termes independents i $B$ és tota la matriu incloent-los)
1. Si $R(A)\neq R(B)$ (com a l'exemple) aleshores la matriu no té cap solució i no podem continuar. 
2. Si $R(A)=R(B)$, aleshores cal comprovar si $R=nº d'incognites$. Si  $R\neq nº \space d'incognites$ aleshores la matriu té solucions però seran infinites. Aquí podrem continuar trobant la relació entre variables ja que el que ens està dient és que una de les variables no la podrem conèixer però això vol dir que podem simplificar el sistema i descobrir-ne algun valor.. 
   El primer pas és trobar els graus de llibertat: 
$$ 
Graus \space de \space llibertat =nº \space incognites - rang
$$
   Un cop els tenim aleshores sabem quantes variables podrem trobar, cada grau de llibertat indica una variable sense valor concret o dependent d'un altre.
3. Si $R(A)=R(B)$ i $R=nº d'incognites$, aleshores finalment podrem resoldre el sistema i trobar solucions concretes a totes les variables.
   Totes les files es poden reescriure com a equacions seguint el mateix principi amb el que les hem convertit en la matriu, si ho hem fet bé tindrem una fila que sera $z=a$ (a no ser que haguem canviat l'ordre de les files).

#### Exemples resolució:
1. Sistema compatible definit:
$$
\begin{cases} 5x-y+z=6 \\ 2x+3y-z=1 \\ x+2y+3z = 4\end{cases}  \quad \Rightarrow \quad \left( \begin{array}{ccc|c} 5&-1&1&6 \\ 2&3&-1&1 \\ 1&2&3&4 \end{array} \right)
$$
	1. Fem Gauss:
$$
\left( \begin{array}{ccc|c} 5&-1&1&6 \\ 2&3&-1&1 \\ 1&2&3&4 \end{array} \right) \quad \Rightarrow \quad \left( \begin{array}{ccc|c} 1&2&3&4 \\ 2&3&-1&1 \\ 5&-1&1&6 \end{array} \right) \quad \Rightarrow \quad \left( \begin{array}{ccc|c} 1&2&3&4 \\ 0&1&7&7 \\ 0&0&63&63 \end{array} \right)
$$
	2. Comprovem si $R(A)=R(B)$ i $R=nº \space d'incognites$ 
$$
R(A) = 3 \quad R(B)=3 \space \checkmark \qquad 3=nº \space d'incognites \space \checkmark
$$
	3. Resolem l'equació:
$$
63z=63 \Rightarrow z=1 \quad y+7z=7 \Rightarrow y=0 \quad x+2y+3z=x+3=4 \Rightarrow x=1
$$
2. Sistema compatible indefinit:
$$
\begin{cases} 3x+2y-z=1 \\ -x+3y-6z=-1 \\ 4x+-y+5z = 2\end{cases}  \quad \Rightarrow \quad \left( \begin{array}{ccc|c} 3&2&-1&1 \\ -1&3&-6&-1 \\ 4&-1&5&2 \end{array} \right)
$$
	1. Fem Gauss:
$$
\left( \begin{array}{ccc|c} 3&2&-1&1 \\ -1&3&-6&-1 \\ 4&-1&5&2 \end{array} \right) \quad \Rightarrow \quad \left( \begin{array}{ccc|c} -1&3&-6&-1 \\ 3&2&-1&1 \\ 4&-1&5&2 \end{array} \right) \quad \Rightarrow \left( \begin{array}{ccc|c} -1&3&-6&-1 \\ 0&11&-19&-2 \\ 0&0&0&0 \end{array} \right)
$$
	2. Comprovem si $R(A)=R(B)$ i $R=nº \space d'incognites$ 
$$
R(A)=2 \quad R(B)=2 \space \checkmark \qquad 2 \neq nº \space d'incognites \space
$$
	3. Simplifiquem l'equació:(tant se val si substituïm $y$ o $z$)
$$
\begin{cases} -x+3y-6z=-1 \\ 11y-19z=-2 \end{cases} \quad \Rightarrow \quad x+\frac 9 {11}z =1
$$
