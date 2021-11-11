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
1. $X\approx N(13,3^2)$
>a. $$P(X<12)=P(\frac{X-13}{3}<\frac{12-13}{3})=P(Z<-0.33)=0.3707$$

>b. $$P(10\le X\le 15)=P(X\le 15)-P(X\le 10)=P(\frac{X-13}{3}\le \frac{15-13}{3})-P(\frac{X-13}{3}\le \frac{10-13}{3})=P(Z\le 0.66)-P(Z\le -1)=0.75-0.16=0.59$$

>c. $$P(X>15)=P(\frac{X-13}{3}>\frac{15-13}{3})=P(Z>0.66)=1-P(Z\le 0.66)=1-0.75=0.25$$
>$Q_3=15$ vidimo iz procentov