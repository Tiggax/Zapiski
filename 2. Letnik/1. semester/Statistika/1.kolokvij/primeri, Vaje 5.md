$$
F(x)=\begin{array}{cc}0;x<-2\\
\frac{1}{4}x+1/2;-2\le x<1
\end$$

$$
\begin{pmatrix}
0.8944272 & 0.4472136\\
-0.4472136 & -0.8944272
\end{pmatrix}
\begin{pmatrix}
10 & 0\\ 
0 & 5
\end{pmatrix}
$$

```chart
type: line
labels: [-3,-2,-1,0,1,1.5,2,3]
series:
	- title: graf1
		data: [0,0,0.25,0.5,0.75,1.5,1.5,1.5]
```

$$f_x(x)=$$

## 2. naloga

$$f(x)=cx^2  ;0<x<2$$
a) $$\int _{-\infty} ^\infty cx^2dx=\int _0^2 cx^2dx=\frac{cx^3}{3}|_0^2=\frac{c8}{3}-0= c*\frac{8}{3}$$
$$c*\frac{8}{3}=1\\ c=\frac{8}{3}$$

>tega nau na kolokviju, sam c) del...

c) $$P(0\le x\le 1)$$
>Fina funkcija(za na listek ;) ):$$P(a\le X\le b)=F(b)-F(a)$$

 $$P(0\le x\le 1)=\frac{1^3}{8}-0=\frac{1}{8}$$
 
 $$P(1\le x\le 2)=\frac{2^3}{8}-\frac{1^3}{8}=\frac{7}{8}$$
 
 ## naloge iz normalne porazdelitve
 >NORMALNA slučajna spremenljivka X $\approx$N(0,1)
 >$$f(x)=\frac{1}{\sigma \sqrt{2x}}e^{-\frac{x-\mu ^2}{2\sigma ^2}}$$

>pomembno: $X\approx$$N(\mu ,\sigma ^2)\to$$Z=\frac{X-\mu}{\sigma}\approx N(0,1)$

3. X$\approx N(65,25)$. 65 predstavlja povprečje srčnega otripa populacije, 25 pa predstavlja varianco -> ($\sigma = 5,\mu=65$)
	a. $P(X\ge 70)$
	>prvo mormo spremenit -> jo standardizirat da bo za iz tabelce brt.
	>$P(X\ge 70)=P(\frac{X-65}{5}\ge \frac{70-65}{5})$ namesto $\frac{X-65}{5}$ lahko pišemo $Z\approx N(0,1)$:
	>$P(Z\ge 1)$
	>**v tabeli so vrednosti $P(Z\ge z)$!**
	>$P(Z\ge z)=1-P(Z<z)$
	>To lahko preberemo iz tabele kot $z$
	>$=1-0.84=0.16$
	
	b. 
	>$P(X\le 70)= 1-P(X> 70)=1-0.16=0.84$ 
	
	c.
	> $P(X\le 120)=P(\frac{X-65}{5}\le \frac{120-65}{5})=P(Z\le 11)=1$
	
	d.
	>$P(70\le X\le 120)=P(X\le 120)-P(X\le 70)=1-0.84=0.16$
	
	d. prvi kvartil porazdelitve
	> $P(X\le x)=0.25$ ali $F(x)=0.25; x=1.kvartil$
	> $P(X\le x)=0.25$
	> $P(\frac{X-65}{5}\le \frac{x-65}{5})=0.25$
	> $P(Z\le \frac{x-65}{5})=0.25$
	> $\frac{x-65}{5}=-0.67$
	> $x-65=-0.67*5$
	> $x=61.65$
	> od te vrednosti ima 25% ljudi večji srčni utrip.
	
4. $X\approx N(13,3^2)$
>a. $$P(X<12)=P(\frac{X-13}{3}<\frac{12-13}{3})=P(Z<-0.33)=0.3707$$

>b. $$P(10\le X\le 15)=P(X\le 15)-P(X\le 10)=P(\frac{X-13}{3}\le \frac{15-13}{3})-P(\frac{X-13}{3}\le \frac{10-13}{3})=P(Z\le 0.66)-P(Z\le -1)=0.75-0.16=0.59$$

>c. $$P(X>15)=P(\frac{X-13}{3}>\frac{15-13}{3})=P(Z>0.66)=1-P(Z\le 0.66)=1-0.75=0.25$$
>$Q_3=15$ vidimo iz procentov

6. neki s pliskavcam... dana je navadna porazdelitev z povprečjem 500. N(500,250)
	a) simetrični interval okrog povprečja ki bo vseboval težo  95% delfinov
	>$P(X\le x_1)=0.025; P(X\le x_2)=0.975$
	>$$P(\frac{X-500}{50}\le \frac{x_1 -500}{50})=0.025$$
	>$$P(Z\le \frac{x_1-500}{50})=0.025$$
	>$$\frac{x_1-500}{50}=-1.96$$
	>$$x_1=402$$

	>$$P(Z\le \frac{x_2-500}{50})=0.975$$
	>$$\frac{x_2-500}{50}=1.96$$
	>$$x_2=598$$
	.
	
	c) peti percentil
	>$$P(X\le x)=0.05$$
	>$$P(Z\le \frac{x-500}{50})=0.05$$
	>$$\frac{x-500}{50}=-1.64$$
	>$$x=418$$
	>5% delfinov je lažjih od 418 lb.

	d) delež delf z težo 500 ali več.$N(500,50^2)$
	> $P(X\ge 500)$
	> $$
	\begin{align}
	Z=\frac{x-500}{500}
	\end{align}
	>$$
	>vidimo iz grafa da je 0,50, ker je X simetrična okoli 500.

	e)
	ne merimo po točkah ker je zvezna 
	> P(X=500)=0

	f) delež delfinov z težo vsaj 450 lb
	> $$
	\begin{align}
	P(z<-1)\\
	1-P(Z<-1)\\
	1-0.1597=0,8413
	\end{align}
	>$$

2. Težo lahko merimo v funtih ali kilogramih. Formula s katero transfrormiramo meritve iz lb v kg je:
>$m(kg)=m(lb)*0.45$
>nove vrednosti bodo zato:
>$$N(500,50^2)\ =>\ N(225,506)$$

3. čas do prve mutacije celic znotraj celične kulture je eksponentno porazdeljena slučajna  spremenljivka. Recimo, da se v povprečju mutacija zgodi po 5 minutah. Izračunaj  verjetnost, da se mutacija zgodi:
	a) prej kot v 3min.
	> $$
	\begin{align}
	P(X<3)=F_X(3)=\\
	=\int_{-\infty}^3\lambda e^{-\lambda t}dt= \\
	=\int_{0}^3\lambda e^{-\lambda t}dt=\\
	=\int_{0}^3 e^{-\lambda}dt=\\
	=e^{-\lambda t}|_0^3=\\
	=1-e^{-3\lambda}\\
	=1-e^{-\frac{3}{5}}
	\end{align}
	>$$

	b) kasneje kot v 6 min.
	> $$
	\begin{align}
	P(X>6)=\\
	1-e^{-\frac{6}{5}}=\\
	=e^{-\frac{1}{5}}	
	\end{align}
	>$$
4. Naj bo X slučajna spremenljivka s funkcijo verjetnosti $$P(X=-1)=P(X=0)=\frac{1}{4};\ P(X=1)=\frac{1}{2}$$
	a) pričakovana vrednost in standardni odklon za slučajno spremenljivko X
	> $$
	\begin{align}
	X:E(X)=\sum_k k*P(X=k)=\\
	-1*\frac{1}{4}+0*\frac{1}{4}+...\\
	=\frac{1}{4}\\
	\\
	\\
	Var(X)=E(X)-E(X)^2
	\end{align}
	>$$
	| $x^2$ | $P(X^2=x^2)$  |
	| ------ | ----------------- |
	| 0         | $\frac{1}{4}$ | 
	| 1         | $\frac{3}{4}$ |
	
	b) pričakovana vrednost, varianca in standarndi odklon za slučajno spremenljivko Y
	> $$
	\begin{align}
	na učilnici
	\end{align}
	>$$

c) kovarianca Cov(X,Y) in korelacijo (X,Y)

| x   | P(X=x) |
| --- | ------ |
| -1  | 1/4    |
| 0   | 1/4    |
| 1   | 1/2    |

> $$
\begin{align}
ne rabmo na kolokviju baje
\end{align}
>$$


## pomembni za kolokvij
### Mlejko
Mlekarna pakira zavitke masla, za katere velja predpis, da je masa normalno poraz-  
deljena s parametroma μ = 250g in σ = 10g. Privzemimo, da se proizvodnja sklada s  
predpisom.
1. kolikšen odstotek zavitkov bo imelo maso vsaj 242g?
> $$
\begin{align}
P(X\ge 242)=\\
P(Z\ge -0,8)=\\
1-P(Z<-0,8)=\\
1-0,21=0,79
\end{align}
>$$

3. Mlekarna dnevno kontrolira zavitke tako, da s slučajno izbiro vzame kontrolni  
vzorec s 25 zavitki, vsak zavitek stehta, iz podatkov pa izračuna vzorčno arit-  
metično sredino. Kolikšen odstotek kontrolnih vzorcev bo imel vzorčno arit-  
metično sredino med 248g in 252,5g?
> $$
\begin{align}
P(248\le \overline{X}_{25}\le 252,5)\\
=P(-1\le Z\le 1,25)=\\
=P(Z\le 1,25)-P(Z\le -1)=\\
=0,8944-0,1587\\
=0,7357
\end{align}
>$$

Vzorčna aritmetična sredina #formula
$$\overline{X}_n=\frac{\sum X_n}{n}$$
$$\frac{\overline{X}_n-\mu}{\frac{\sigma}{\sqrt n}}\approx N(0,1)$$


4. Predpostavimo, da je vsebnost beljakovin v mleku, ki ga mlekarna odkupuje od svojih  
proizvajalcev, normalno porazdeljena s povprečno vrednostjo 3,15% in standardnim  
odklonom 0,30%.  
V kontroli kakovosti mleka mlekarna od vsakega proizvajalca vzame po 4 stekleničke  
mleka in za vsako stekleničko ugotovi vsebnost beljakovin. Iz teh štirih števil izračuna  
aritmetično sredino.  
Mlekarna od proizvajalcev mleka, pri katerih je vzorčna aritmetična sredina manjša  
od 3% odkupuje mleko po zniˇzani ceni, za mleko z vzorčno aritmetično sredino med  
3,00% in 3,20% plačuje normalno ceno, za mleko z vzorčno aritmetično sredino nad  
3,20% pa plačuje zvišano ceno.  
Izračunajte od koliko % proizvajalcev bo mlekarna odkupovala mleko po zniˇzani,  
normalni in zvišani ceni
> $$
\begin{align}
\frac{\overline{X}_4-3,15}{\frac{0,3}{\sqrt4}}\approx N(0,1)\\
\\
P(\overline{X}_4<3)=\\
P(Z<\frac{3-3,15}{\frac{0,3}{\sqrt4}})=\\
P(Z<-1)=0,16
\end{align}
>$$

> $$
\begin{align}
P(\overline{X}_4>3,2)=\\
P(Z>\frac{3,2-3,15}{\frac{0,3}{\sqrt4}})=\\
P(Z>\frac{0,05*2}{0,3})=\\
P(Z>0,33)=\\
=1-P(Z\le 0,33)=\\
=1-0,63=\\
=0,37
\end{align}
>$$

7. V tabeli je navedeno število prometnih nesreč na cestah v Sloveniji  
in število smrtno ponesrečenih v teh nesrečah.  

| Leto | število prometnih nesreč | število smrtno ponesrečenih | indeksi za 1996 | verižni indeksi | $S_{t/t-1}$ |
| ---- | ------------------------ | --------------------------- | --------------- | --------------- | ----------- |
| 1992 | 5.882                    | 492                         | 126,5           | /               | /           |
| 1993 | 6.290                    | 493                         | 126,7           | 100,2           | 0,2         |
| 1994 | 6.586                    | 505                         | 129,8           | 102,4           | 2,4         |
| 1995 | 6.540                    | 415                         | 106,7           | 82,2            | -17,8       | 
| 1996 | 6.348                    | 389                         |                 |                 |             |
| 1997 | 6.951                    | 358                         |                 |                 |             |
| 1998 | 5.864                    | 309                         |                 |                 |             |

Za število smrtno ponesrečenih izračunajte: indekse z osnovo 1996, verižne indekse in  
stopnje rasti.
