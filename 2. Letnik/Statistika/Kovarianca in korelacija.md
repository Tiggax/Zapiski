# Kovarianca
$Var(x)$ (Varianca) je merilo razpršenosti slučajne spremenljivke X okoli pričakovane vrednosti $\mu =E(X)$
**Kovarianca in korelacija** merita povezanost dveh slučajnih spremmenljivk
>naj bosta X in Y sličajni spremenljivki $\mu _x=E(X)$ in $\mu _y=E(X)$

**Kovarianca** je :
>$$Cov(X,Y)=E(X,Y)-E(X)E(Y)$$

```ad-note
collapse:T
title: Primer:


| k   | P(X=k) |
| --- | ------ |
| -1  | 0.2    |
| 0   | 0.4    |
| 1   | 0.4    |


| k   | P(X=k) |
| --- | ------ |
| -1  | 0.2    |
| 0   | 0.4    |
| 1   | 0.4    |

Funkcija verjetnosti za spremenljivko Y je:

| 1   | 0.4 |
| --- | --- |
| 2   | 0.6 |

>$$E(Y)=1*0.4+2*0.6=1.6$$

Za spremenljivko XY je funkcija verjetnosti:

>$$P(XY=-2)=P(X=-1)=0.2$$
>$$P(XY=0)=P(X=0)=0.4$$
>$$P(XY=2)=P(X=1)=0.4$$

>$$E(XY)=(-2)+0.2'0*0.4+2*0.4$$
>...
>$$Cov(X,Y)=0.08$$


```

