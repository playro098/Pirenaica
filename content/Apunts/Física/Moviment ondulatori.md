### Definició:
Si llencem una pedra a l'aigua aquesta genera una pertorbació en la superficie de l'aigua que és transmet per tota la seva superficie en forme de circumferències concèntriques. Si en aquesta aigua col·loquem un tap de suro aquest es veurà afectat per un moviment harmonic simple. El punt d'origen de la pertorbació és el focus.
Hi ha diferents tipus d'ona en base a multiples criteris:
1. **Segons el nombre de dimensions en que es propaguen**
	1. Unidimensionals: Ones a través d'una corda
	2. Bidimensionals: Ones a través de superficies liquides
	3. Tridimensionals: Ones de so, llum i sota la superficie de l'aigua
2. **Segons el medi de propagació:**
	1. Mecàniques: Necessiten un medi material per propagar-se com l'aigua o l'aire (el so).
	2. Electromagnètiques: Es poden propagar al buit (llum, ràdio, raigs X).
3. **Segons la direcció relativa de la propagació i l'oscil·lació de les partícules:
	1. Longitudinals: les partícules vibren en la mateixa direcció de propagació de l'ona (so, vibració d'una molla)
	2. Transversals: les partícules vibren en una direcció perpendicular a la propagació de l'ona (vibració d'una corda fixa per un extrem.
### Elements d'una ona
Una ona es transmet més ràpidament com més alta és la densitat del medi.
#### Termes:
1. **Velocitat de fase:** Velocitat amb què es transmet la pertorbació. Cal distingir-la de la velocitat de vibració de les partícules del medi que es produeix la pertorbació.
2. **Front d'ona:** Conjunt de punts del medi on arriba la pertorbació en un moment determinat
3. **Raigs:** Lins perpendiculars al front que marquen les direccions d'avenç
4. **Crestes:** Punts més alts de l'ona
5. **Valls:** Punt més baixos

### Ones Harmòniques:
Pertorbacions que causen un MHS en les partícules del medi en el que es transmeten. En aquests exercicis haurem de trobar l'equació que defineix el moviment de la partícula en qualsevol interval de temps. 
Per saber on és el focus (partícula on s'inicia el moviment, on $x=0$)
$$
y = A·cos(\omega·t)
$$
Per conèixer la posició d'una partícula que es troba en el mateix moviment harmonic però amb $x=a$, i per tant més endavant en la ona, farem servir la equació següent.
$$
y = A·cos(\omega ·t')
$$
En realitat t' és $\Delta t$, és a dir la diferencia de temps. Fem servir la següent equació perquè al parlar d'ones ens és molt més útil que $t_x-t_0$, tot i ser tècnicament el mateix. La relació entre $t'$ i $t$ és la següent:
$$
t'=t-\frac x v
$$
Per tant l'equació final sera la següent:
$$
y=A·cos[\omega·(t-\frac x v)]
$$
Però casi mai ho veurem escrit així, la manera més comuna de veure això escrit sera fent servir el nombre d'ona ($k$):
$$
k=\frac \omega v \qquad y=A·cos(\omega·t-k·x)
$$
Si recordem abans quan hem descrit la longitud d'ona sabem que:
$$
\lambda = v · T
$$
I per tant també podem escriure la següent expressió:
$$
y=A·cos(\omega·t-k·x)=A·cos[2\pi·(\frac {t}{T}- \frac {x}{\lambda})]
$$
Cal tenir en compte que si l'ona viatja de dreta a esquerra haurem de canviar el signe dins del parèntesi del cosinus.
Recordeu el nombre d'ona o $k$ que hem vist abans? Doncs es pot relacionar directament amb la longitud d'ona:
$$
k=\frac{2\pi}{\lambda}
$$
Això ens permet definir $k$ com el nombre de longituds d'ona complets en una distancia de $2\pi$ metres.
L'ona harmònica pot tenir una fase inicial i s'escriu:
$$
y(x,t)=A·sin (\omega·t-kx+\alpha)
$$
Recordem que podem canviar sinus per cosinus i viceversa sumant o restant $\frac{\pi}{2}$ al seu angle. Aquesta equació es fa servir quan treballem amb ones que avancen amb el temps. Totes ho fan però pocs problemes ens demanaran les dades necessaries per fer-la servir.
### Magnituds importants:
Període:
$$
T = \frac {2\pi} {\omega}
$$