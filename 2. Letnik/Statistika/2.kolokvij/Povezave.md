

- **odvisnost**
	- 
- **povezanost** oz. korelacija slučajnih spremenljivk
	- > v navadi gre za povezonost dveh spremenljivk od tretje

# Odvisnost
## Regresija
prilagajanje neke funkcije nekim podatkom.
imamo $x$ in $y$. $x$ je neodvisna spremenljivka, $y$ pa odvisna.

```chart
type: line
labels: [0,1,2,3,4,5,6,7]
series:
  - title: y
    data: [2,3,4,5,6,7,8,9,]
tension: 0.2
width: 80%
labelColors: false
fill: false
beginAtZero: false
```
predstavimo jo z $\ovearched Y= a + bX$

 s tem iščemo **regresijsko premico** $$\overarch Y=a+bX$$, ki se najbolje prilega podatkom. to pomeni, da morajo biti odkloni $y_i-\overarch Y$ od premice čim manjši. ker so +- je smiselno pogledati kvadrirane odklone, in premico dloločimo tako, da je **vsota kvadriranih odklonov** minimalna:
 $$\min\sum_{i=1}^n(y_i-\overarch y_i)^2=\min\sum_{i=1}^n(y_i-ax_i-b)^2$$
 označimo aritmetični sredini danih podatkov. 
 $$b=\frac{\sum_{i=1}^n(x_i-\overline x)(y_i-\overline y)}{\sum_{i=1}^n(x_i -\overline x)^2}=\frac{\sum_{i=1}^nx_iy_i-n\overline x\overline y}{\sum_{i=1}^n x_i^2-n\overline x^2}$$
 
 intepretacija podatkov regresijske premice

### Kvocient determinacije
regresijski modeli različno dobro zajemajo dane podate





