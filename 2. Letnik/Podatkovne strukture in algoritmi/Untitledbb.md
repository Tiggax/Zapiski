## NALOGA
imamo ključe med  neki {0,1}
$x_1$=1111110
$x_2$=0001010110
$x_3$=0110000
$x_4$=011110

```mermaid
graph TB;
A[1]-- 0 ---B
B[2]-- 0 ---C[x2]
A-- 1 ---D
D-- 0 ---H
H-- 1 ---M
D-- 1 ---I
B-- 1 ---E
E-- 0 ---F
E-- 1 ---G
G-- 0 ---J
G-- 1 ---K

```
Stisnit po plasteh ->

```mermaid
graph TB;
subgraph ena
A 
end
subgraph dve
D
B
end
subgraph tri
C
E
H
I
end
subgraph stiri
F
G
M
end
A[1]-- 0 ---B
B[2]-- 0 ---C[x2]
A-- 1 ---D
D-- 0 ---H
H-- 1 ---M
D-- 1 ---I
B-- 1 ---E
E-- 0 ---F
E-- 1 ---G
G-- 0 ---J
G-- 1 ---K

```
vsak nivo je en $2^n$ moznih odgovorov aka:
prvi nivo sta mozna 0 ali 1
drugi nivo so mozni 00 01 10 ali 11

## ključi
za n ključev 
imamo nekaj n ključev za $\epsilon$={0,1} 
a) neki neki da ne bo o+nobenega polja/vektorja z drugimi besedami bi za vsako stiskanje po poteh bila gostota vedno prenizka.
kakšne vrdnosti morjo met ključi da ne bo nobenega stiskanja?
> ali vsi začnejo z 0 ali pa z 1

recimo da se vsi ključi začnejo z 0

```mermaid
graph LR
A---B
B---C
B---D
D---E
D---F
```
v primeru z 
```mermaid
graph LR
B---C
B---D
D---E
D---F
```
se pravi če zelimo da ne bo stiskanja se morajo vsi začeti z 0 ali z 1.
## Dvojiška iskalna drevesa
podoben slovarju? 
je neka struktura ki operira z elementi
Ima:
- iskanje
- brisanje
- vstavljanje
imamo elemente ki jih vstavljamo:
**Ključ** in **podatek**

### Vstavljanje
PRIMER:
mamo : 30,48,58,40,24,26,11,13
```mermaid
graph LR
A[30]
B[48]
C[58]
D[40]
E[24]
F[26]
G[11]
H[13]
A---B
B---C
A---E
B---D
E---F
E---G
G---H
```
### Brisanje

Zbrišemo 58
```mermaid
graph LR
A[30]
B[48]
D[40]
E[24]
F[26]
G[11]
H[13]
A---B
A---E
B---D
E---F
E---G
G---H
```
---
uporabljamo primerjalni primer.

### Pregled
