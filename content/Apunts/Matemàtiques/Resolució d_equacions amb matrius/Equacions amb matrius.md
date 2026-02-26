Suposem que ens donen un sistema d'equacions amb tres o més variables:
$$
\begin{cases} x-y+z=0 \\-3x+2y=1\\ -5x+2y+4z=12 \end{cases}
$$
El podem convertir en una matriu posant tots els numeradors de cada variable en una matriu directament, recordem mantenir l'ordre de variables i separem per una ratlla la columna de termes independents, Aquesta matriu sera la base per resoldre el sistema.
$$
B_{3x4}=\left(
\begin{array}{ccc|c}
1 & -1 & 1 & 0 \\
-3 & 2 &  0 & 1 \\
-5 & 2 &  4 & 12
\end{array}
\right)
\qquad A_{3x3}=\begin{pmatrix} 1 & -1 & 1 \\ -3 & 2 &  0\\ -5 & 2 &  4\end{pmatrix}
$$
Aquesta matriu sencera sera $B$, la matriu $A$ sera la mateixa però excloent la columna de termes independents. Tenim multiples opcions per resoldre els sistemes:
![[Mètode de Gauss]]
