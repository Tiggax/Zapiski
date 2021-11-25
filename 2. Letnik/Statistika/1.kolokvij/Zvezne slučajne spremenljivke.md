# Zvezne slučajne spremenljivke
lahko zavzemajo kontinuum vrednosti
npr: $[a,b],R,R^n,...$
Funkcija gostote verjetnosti  mora biti:
>- $f>=0$
>- je odsekoma zvezna
>- $\int(inf,inf)f(x)dx=1$
>če ima sučajna spremenljivka X gostoto f, je:
>$P(a<=X<=b)=\int(a,b)f(x)dx$

nikoli ne merimo točne vrednost (P(X=x)) ker je ta vedno 0, ampak merimo na intervalih($P(X\le x)$)

---
## Porazdelitvena funkcija
slučajne spr. X z gostoto f je:
$F(x)=P(X<=x)=int(-inf,X)f(s)ds$
F(x) je verjetnost, da sučajna spremenljivka X zavzame vrednost do največ x
Za porazdelitveno funkcijo velja:
- F je naraščajoča
- $lim _{x\to\infty} F(x)=1$
- $lim_{x\to\infty} F(x)=0$
- $F'(x)=f(x)$
**Primer:**
>$$f(x)={(1 za 0<=x<=1),(0 sicer)}$$
porazdelitvena je:

---
## Kvantili za zvezne slučajne spremenljivke
naj bo X zvezna slučajna spremenljivka s porazdelitveno funkcijo F.
$\color{red}p-kvantil$ $(0<=p<=1)$ za spremenljivka+o X je vrednost $x_(p)$, za katero velja:
$P(X<=x_p)=p$
oz:
$F(x_p)=p$
**Primer:**
slučajna spr. X lahko zavzame vred: $[0,\inf)$ in ima funcijo: $F(x)=\frac{x}{1+x}$
- funkcija gostote:
	$f(x)=F'(x)=\frac{1}{(1+x)^2}$
- verjetnost, Da X zavzame vrednost na intervalu $[1,2)$ je:
	$P(1<=X<=2)=F(2)-F(1)=\frac{2}{3}-\frac{1}{2}=\frac{1}{6}$
- Mediana je vrednost Me, za katero $F(Me)=0.5$, torej $Me=1$
- $Q_{0.25}=\frac{1}{3}$

---
## Pričakovane vrednosti in varianca
**pričakovana vrednost** je:
$E(X)=\int\limits_{-inf}^{inf}xf(x)dx$
**varianca** slučajne spremenljivke X, s pričakovano vrednostjo $u=E(X)$ je:
$Var(X)=E((X-u)^2)=E(X^2)-E^2(X)$
**Pimer:**
Slučajna spremenljivka X lahko zavzame vrednosti v $[0,1)$ in ima funkcijo gostote $f(x)=6x(1-x)$. Izračunajmo $E(X)$ in $Var(X)$

---
## Eksponentna porazdelitev $Exp(\lambda)$
Gostota slučajne spremenljivke X z eksponentno porazdelitvijo s parametrom $\lambda(X~Exp(\lambda))$ je:
$f(x)={(\lambda e^{-\lambda x} za x>=0),(0za)}$

---
## Gausova porazdelitev
ima dva parametra $X~N(\mu, \sigma^2)$

---
## Standardna normalna slučajna spremenljivka
Z~N(0,1) ima funkcijo gostote:
$f(x)=\frac{1}{\sqrt{2\pi}}e^{\frac{-x^2}{2}}$

**Primer:**
Naj bo X~N(0,1). s pomočjo tabele določimo:
- $P(X<=1.05)$
- $P(X>=2)$ == $P(X=<-2)$ na tabeli
- $P(-1<=X<=2.65)$=$P(X<=2.65)-P(X<=-1)$=$0.9960-0.1587$=$0.8373$
- $Q_{0.25}$=iz tabele ~ 0.67
- Mediana= v točki 0
- $Q_{7/10}$~ 0.52
**Primer:**
Sistolični krvni tlak X je v popilaciji normalo porazdeljen s pričakovano vrednostjo $\mu=112$ in standardnim odklonom $\sigma = 10$
Torej X~$N(\mu,\sigma^2)$ in Z=$\frac{X-p}{\sigma}~N(0,1)$
- $P(\frac{X-112}{10}<=\frac{122-112}{10})$=
$P(Z<=1)$=
0.841
- $P(102<=X<=122)$=
=$P(\frac{102-112}{10}<=\frac{X-112}{10}<=\frac{122-112}{10})$=
=$P(-1<=Z<=1)$=
=$P(Z<=1)-P(Z<=-1)$=
=$0.8413-0.1587$=
=$0.6826$
- $P(X>140)$=
=$P(\frac{X-112}{10}>\frac{140-112}{10})$=
=$P(Z>2.8)$=
=$P(Z<-2.8)$=
=$0.0026$