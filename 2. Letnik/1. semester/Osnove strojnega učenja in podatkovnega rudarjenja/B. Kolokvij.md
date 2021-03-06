# Kolokvij naloga B

| I   | D        | E   | F   | G_d | G   | C   |
| --- | -------- | --- | --- | --- | --- | --- |
| 100 | 2000,00  | N   | C   |     | 3   | T   |
| 101 | 2003,328 | N   | A   |     | 5   | F   |
| 102 | 2012,284 | Y   | B   |     | 10  | T   |
| 103 | 2007,163 | N   | A   |     | 9   | T   |
| 104 | 2002,497 | N   | C   |     | 11  | F   |
| 105 | 2015,175 | Y   | C   |     | 10  | F   |
| 106 | 2020,000 | Y   | C   |     | 4   | F   |
| 107 | 2018,459 | Y   | A   |     | 8   | T   |
| 108 | 2013,646 | Y   | B   |     | 19  | T   |
| 109 | 2019,005 | N   | B   |     | 7   | T   |
| 110 | 2008,205 | Y   | A   |     | 14  | F   |

| I   | D(ni v KSP)  | E   | F   | G_d | G   | C_nb | C_od |
| --- | ------------ | --- | --- | --- | --- | ---- | ---- |
| 200 | 21.2.2011    | N   | A   |     | 9   |      |      |
| 201 | 17.6.2013    | N   | C   |     | 11  |      |      |
| 202 | **3.5.2012** | Y   | B   |     | 2   |      |      |


1. Pretvorite vrednosti atributa D v primerih 200, 201 in 202 v KSP format (prestopno leto je odebeljeno)! Rezultat zaokrožite na tri decimalna mesta! (10 točk)  
  
2. Skicirajte box-plot za vrednosti atributa G (upoštevajte le primere z zaporedno številko med vključno  
100 ter vključno 110)! (10 točk)  
>po vrsti: 3,4,5,7,8,9,10,10,11,14,19
>Mediana: 9 = $(n+1)+0.5$
>$Q_{0,25}=\ 5$
>$Q_{0,25}=\ 11$
>```
>insert boxplot
>```
  
3. Diskretizirajte atribut G na 4 enako visoke intervale (upoštevajte le primere z zaporedno številko med vključno 100 ter vključno 110)! Nov atribut G_d naj ima vrednosti G1, G2, G3 in G4. Skicirajte histogram! (10 točk)  
  >po vrsti: 3,4,5,7,8,9,10,10,11,14,19


```chart
type: bar
labels: [a,b,c]
series:
	- title: graf1
		data: [3,4,5,7,8,9,10,10,11,14,19]
```
| intervali | vrednost |
| --------- | -------- |
| G1        | 3,4,5    |
| G2        | 7,8,9    |
| G3        | 10,10,11 |
| G4        | 14,19    | 


  | G_d | G   |
  | --- | --- |
  | G1  | 3   |
  | G1  | 5   |
  | G3  | 10  |
  | G3  | 9   |
  | G2  | 11  |
  | G3  | 10  |
  | G1  | 4   |
  | G2  | 8   |
  | G4  | 19  |
  | G2  | 7   |
  | G4  | 14  |



4. Uporabite algoritem OneR za klasifikacijo primerov s poznanim razredom! Upoštevajte le atribut E. Skicirajte (eno-nivojsko) odločitveno drevo! Kolikšna je napaka tega klasifikatorja? (15 točk)  

| $\\_E^F$ | T   | F   | napaka |
| -------- | --- | --- | ------ |
| n        | 3   | 2   | 2      |
| y        | 3   | 3   | 3      |
| ---      | --- | --- | ---    |
|          |     |     | 5      |
  
| $\\_E^F$ | T   | F   | napaka |
| -------- | --- | --- | ------ |
| A        | 2   | 2   | 2      |
| B        | 3   | 0   | 0      |
| C        | 1   | 3   | 1      |
| ---      | --- | --- | ---    |
|          |     |     | 3      |

  
  
  
5. Uporabite algoritem Naivni Bayes za klasifikacijo primerov z neznanim razredom! Upoštevajte le atributa E in F. Pri izračunu verjetnosti uporabite Laplace-ovo oceno (25 točk)  
| stolpec | T   | F   |
| ------- | --- | --- |
| N       | 4/8 | 3/8 |
| Y       |     |     |
| ---     | --- | --- |
| A       |     |     |
| B       |     |     |
| C       |     |     |
  
  
  200: $$L('T')=E(N)*F(A)*C$$
  $$L('T')=4/8*3/9*7/13$$
  
  202: $$L(T)=3/8*4/9*7/13=0,1197$$
  $$L(F)=4/8*1/8*6/13=0,0330$$
  
  
  
  
6. Zgradite prvi nivo odločitvenega drevesa (korensko vozlišče) po metodi TDIDT (algoritem ID3) pri čemer upoštevajte le atribute E, F in G_d. Kot mero za »čistost« podmnožic uporabite informacijski prispevek (information gain). Tako dobljeno »delno« odločitveno drevo narišite ter ga uporabite za klasifikacijo primerov z neznanim razredom!

| I   | D        | E   | F   | C   | G_d | G   |
| --- | -------- | --- | --- | --- | --- | --- |
| 100 | 2000,00  | N   | C   | T   | G1  | 3   |
| 101 | 2003,328 | N   | A   | F   | G1  | 5   |
| 102 | 2012,284 | Y   | B   | T   | G3  | 10  |
| 103 | 2007,163 | N   | A   | T   | G3  | 9   |
| 104 | 2002,497 | N   | C   | F   | G2  | 11  |
| 105 | 2015,175 | Y   | C   | F   | G3  | 10  |
| 106 | 2020,000 | Y   | C   | F   | G1  | 4   |
| 107 | 2018,459 | Y   | A   | T   | G2  | 8   |
| 108 | 2013,646 | Y   | B   | T   | G4  | 19  |
| 109 | 2019,005 | N   | B   | T   | G2  | 7   |
| 110 | 2008,205 | Y   | A   | F   | G4  | 14  |

```mermaid
graph TB
subgraph Y[E]
	A[E]-- N ---B[T,T,T<br>N,N]
	A-- Y ---B1[T,T,T<br>N,N,N]
end
subgraph X[F]
	C[F]-- A ---D[t,t<br>N,N]
	C-- B ---D1[T,T,T]
	C-- C ---D2[T<br>F,F,F]
end
subgraph G_d
	E[G_d]-- G1 ---F[T<br>F,F]
	E-- G2 ---F1[T,T,T]
	E-- G3 ---F2[T<br>F,F]
	E-- G4 ---F3[<br>F]
end
```
```mermaid
graph TD
subgraph Dr[drevo]
	G[F]-- A ---H[T]
	G-- B ---H1[T]
	G-- C ---H2[F]
end
```
information gain: $$IBS=\frac{5}{11}\log_2\frac{5}{11}-\frac{6}{11}\log_2 \frac{6}{11}=0,994$$