### Principi de superposició:

### Ones coherents:
Nosaltres només estudiarem interferències entre dues ones coherents, és a dir, amb la mateixa amplitud. Estudiarem com es troben en un punt i quina és la seva diferencia en ell.
$$
y_{(x,t)}=A·sin(\omega·t-k·x+\alpha_0)
$$
I en un punt, sabent que les ones es sumen, tindrem que:
$$
y=y_{1}(r_1,t)+y_{2}(r_2,t)=A_0[sin(\omega·t-k·r_1)+sin(\omega·t-k·r_2)]
$$
A través d'identitats trigonomètriques diem el següent:
$$
sin(\alpha)+sin(\beta)=2cos \left( \frac{\alpha - \beta}{2} \right)·sin\left( \frac{\alpha + \beta}{2} \right)
$$
I per tant diem:
$$
2A_0·cos\left(\frac{k(r_2-r_1)}{2} \right)·sin\left(\omega·t·\frac{k(r_1+r_2)}{2} \right)
$$
És curios observar que només depen del temps la segona part de l'equació, donant una equació de moviment ondulatori i això és perquè la amplitud del punt sera realment tot el primer bloc, el valor màxim d'$A$ per tant sera $2A_0$.

Les interferències poden ser constructives o destructives i és classifiquen segons el valor d'$A$
Si $A_{màx}=2A_0$ és constructiva i vol dir que:
$$
cos \left( \frac{\pi(r_2-r_1)}{\lambda} \right)=\pm1
$$
És a dir que si amplitud és 
$$
2A_0·cos \left( \frac{\pi(r_2-r_1)}{\lambda} \right)=\pm1
$$
Aquesta sera màxima i la interferència en aquest pun constructiva.
Per contrapartida si:
$$
cos \left( \frac{\pi(r_2-r_1)}{\lambda} \right)=0
$$
L'amplitud serà minima.
El que aquestes equacions ens acaben indicant és que treballarem amb dues equacions que mesuren la distancia entre diferents punts d'interferència constructiva:
$$
r_2-r_1=n\lambda \quad n=0,\pm1,\pm2,...
$$
I destructiva:
$$
r_2-r_1=(2n+1)\frac{\lambda}{2}
$$





### Ones estacionàries:
Es creen a través del xoc de dues ones iguals. Sol passar quan una ona xoca contra una paret i de tornada es troba amb ella mateixa.
Per entendre-la cal calcular les interferències entre dues ones idèntiques superposades. Ja que és el que fan al rebotar. L'ona que rebota només pateix un canvi, sumem $\pi$ al seu angle, invertint-la.
Per tant:
$$
A_i=-A_r \qquad A_r=-A_i=-A_0
$$


Nodes: Són punts de vibració nul·la i es situen a una distancia de:
$$
WIP
$$
Les ones sempre acabaran formant patrons que dependran de $n$, amb $n=1$ sent la ona principal, podem anar complicant cada cop més l'ona.

Expressió dels Harmonics en un tub semiobert:
$$
\lambda_{2n+1}=\frac{4L}{2n+1}=0,1,2,3..
$$

### Energia del moviment ondulatori:
Si recordem:
$$
E=E_c+E_p
$$
$$
E=E_{p \space màx}= \frac{1}{2}m(\omega A)^2=\frac{1}{2}m(2\pi fA)^2=2\pi^2mf^2A^2
$$
Per continuar cal definir l'intensitat d'energia transmesa, que és la potència mitjana per unitat de superfície perpendicular a la direcció de propagació.
$$
I=\frac{Potència}{Superfície}=\frac{\Delta E}{S·\Delta t} \quad (W/m^2)
$$
Aquí podem fer servir un truc per fer el següent:
$$
I=\frac{\Delta E}{S·\Delta t}·\frac{\Delta r}{\Delta r} = \frac{\Delta E}{V}·v
$$
On $V$ és un volum. Podem continuar i fer servir l'expressió de l'energia que hem trobat abans per acabar fent la següent equació:
$$
2\pi^2·\rho·v·f^2·A^2=E
$$
