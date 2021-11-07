## Frekvenčna porazdelitev
če ima $X$ spremenljivka končen nabor vrednosti, npr: $a_1,a_2,...,a_n$
število pojavljan vrednosti $a_j,(j=1,...,n)$ je <span style="color:red">frekvenca</span> enote $a_j$
>$f_j=\#(X=a_j)$

**Relativna frekvenca**j-te enote je:
>$f^0_j=\frac{f_j}{\sum^n_1f_n}$
>ali izražena v odstotkih:
>$f_j\%=100*\frac{f_j}{\sum^n_1f_n}$

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

```chart
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