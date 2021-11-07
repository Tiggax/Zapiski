## Frekvenčna porazdelitev
če ima $X$ spremenljivka končen nabor vrednosti, npr: $a_1,a_2,...,a_n$
število pojavljan vrednosti $a_j,(j=1,...,n)$ je <span style="color:red">frekvenca</span> enote $a_j$
>$f_j=\#(X=a_j)$

**Relativna frekvenca**j-te enote je:
>$f^0_j=\frac{f_j}{\sum^n_{k=1}f_k}$
>ali izražena v odstotkih:
>$f_j\%=100*\frac{f_j}{\sum^n_{k=1}f_k}$

predstavimo jih z histogramom ali tortnim diagramom. 
```ad-example
collapse: T
title: Primer:

60 naključno izbranih povprašamo po njihovem najljubšem  
okusu sladoleda. Dobimo naslednje odgovore:  
V, Č, J, V, P, J, L, Č, P, V, J, Č, V, P, Č, L, Č, J, Č, V, P, L, V, Č, P, Č, J, Č, Č, P, J, Č, V, L, Č, P, V, Č, Č, L, J,Č, P, V, V, J, L, V, P, Č, Č, P, Č, V, L, Č, V, J, V, P  
Č = čokolada, V = vanilija, J = jagoda, L= lešnik, P = pistacija

---
| Okus      | $f_j$ | $f_j\%$ |
| --------- | ----- | ------- |
| Čokolada  | 19    | 32      |
| Vanilija  | 14    | 23      |
| Jagoda    | 9     | 15      |
| Lešnik    | 7     | 12      |
| Pistacija | 11    | 18      |

```chart
type: bar
labels: [Čokolada,Vanilija,Jagoda,Lešnik,Pistacija]
series:
  - title: $f_j$
    data: [19,14,9,7,11]
  - title: $f_j\%$
    data: [32,23,15,12,18]
width: 80%
beginAtZero: true

```
```chart
type: pie
labels: [Čokolada,Vanilija,Jagoda,Lešnik,Pistacija]
series:
  - title: $f_j$
    data: [19,14,9,7,11]
  - title: $f_j\%$
    data: [32,23,15,12,18]
width: 80%
beginAtZero: true
```
če imajo urejenostne ali številske spremenljivke $X$ *končen nabor* vrednosti, jih lahko <span style="color:red">uredimo po velikosti</span> npr.:$a_1<a_2<a_3<...<a_n$ ter poleg frekvenc še izračunamo [[#^3743fe|kumulativne frekvence]].
## Kumulativne frekvence
Kumulativne frekvence izračunamo:
>$F_j=\#(X\le a_j)=\sum^j_{n=1}f_n$
>____
>$F_j$ je število enot ki imajo največ vrednost $a_j$

Relativne kumulativne frekvence
>$F_j\%=100*\frac{F_j}{\sum^n_{k=1}f_k}$

```ad-example
title:Primer:
collapse: T

| Ocene  | $f_j$ | $f_j$% | $F_j$ | $F_j$% |
| ------ | ----- | ------ | ----- | ------ |
| 5      | 22    | 29.3   | 22    | 29.3   |
| 6      | 17    | 22.7   | 39    | 52     |
| 7      | 14    | 18.7   | 53    | 70.7   |
| 8      | 9     | 12     | 62    | 82.7   |
| 9      | 6     | 8      | 68    | 90.7   |
| 10     | 7     | 9.3    | 75    | 100    |
| Skupaj | 75    |        |       |        |
```chart
type: bar
labels: [5,6,7,8,9,10,Skupaj]
series:
  - title: $f_j$
    data: [22,17,14,9,6,7,75]
  - title: $f_j$%
    data: [29.3,22.7,18.7,12,8,9.3,]
  - title: $F_j$
    data: [22,39,53,62,68,75,]
  - title: $F_j$%
    data: [29.3,52,70.7,82.7,90.7,100,]
width: 80%
beginAtZero: true
```
### Dodatne lasnosti razredov
ko je možnih vrednosti veliko, jih običajno razdelimo na intervale. v primeru da so spremenljivke razdeljene v K intervalov, potem frekvenčno porazdelitev opremimo še s:
- **spodnjo in zgornjo mejo razredov** tako da:
	$x_{i,min}$ in $x_{i,max}$ za $i=1,...,K$
	>$x_{i,max}=x_{i+1,min}$
	Zgornja meja razreda je spodnja meja naslednjega.
- **širino razreda**
	>$d_i=x_{i,max}-x_{i,min}$
	v primeru da so širine razredov različno velike ,podatki po razredih niso primerljivi. Tedaj za vsak razred izračunamo **gostoto frekvenc**
	$g_i=\frac{f_i}{d_i}$
	
- **sredina razreda**
	>$x_i=\frac{x_{i,max}+x_{i,min}}{2}$
	>--

```ad-example
collapse: T
title: Primer:
Za 30 učencev imamo podatke oštevilu ur odsotnosti v  
zadnjem šolskem letu:  
70,54,29,73,72,47,41,43,59,97,43,52,67,42,73  
84,74,60,80,71,42,69,37,64,78,63,59,72,72,69  
Odločimo se za razrede: 20 −39,40 −59,60 −79,80 −99 in zapišemo  
frekvenčno tabelo
---
| Odsotnost (h) | xi,min | xi,max | di  | xi   | fi  | fi % | Fi  | Fi % |
| ------------- | ------ | ------ | --- | ---- | --- | ---- | --- | ---- |
| 20-39         | 19.5   | 39.5   | 20  | 29.5 | 2   | 6.7  | 2   | 6.7  |
| 40-59         | 39.5   | 59.5   | 20  | 49.5 | 10  | 33.3 | 12  | 40   |
| 60-79         | 59.5   | 79.5   | 20  | 69.5 | 15  | 50   | 27  | 90   | 
| 80-99         | 79.5   | 99.5   | 20  | 89.5 | 3   | 10   | 30  | 100  |

```chart
type: bar
labels: [20-39,40-59,60-79,80-99]
series:
  - title: xi,min
    data: [19.5,39.5,59.5,79.5]
  - title: xi,max
    data: [39.5,59.5,79.5,99.5]
  - title: di
    data: [20,20,20,20]
  - title: xi
    data: [29.5,49.5,69.5,89.5]
  - title: fi
    data: [2,10,15,3]
  - title: fi %
    data: [6.7,33.3,50,10]
  - title: Fi
    data: [2,12,27,30]
  - title: Fi %
    data: [6.7,40,90,100]
width: 80%
beginAtZero: true
```
podatke lahko poleg histograma predstavimo še s poligonom ali pa z ogivo, pri kateri na abscisno os narišemo zgornje meje razredov, na ordinatno pa pripadajoče relativne kumulativne frekvence.
