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
> $$
\begin{align}
f
\end{align}
>$$