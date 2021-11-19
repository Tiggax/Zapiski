| I   | D        | E   | F   | G_d | G   | C   |
| --- | -------- | --- | --- | --- | --- | --- |
| 100 | 2000,00  | N   | C   |     | 3   | T   |
| 101 | 2003,328 | N   | A   |     | 5   | F   |
| 102 | 2012,284 | Y   | B   |     | 10  | T   |
| 103 |          |     | A   |     | 9   | T   |
| 104 |          |     | C   |     | 11  | F   |
| 105 |          |     | C   |     | 10  | F   |
| 106 |          |     | C   |     |     | F   |
| 107 |          |     | A   |     |     | T   |
| 108 |          |     | B   |     |     | T   |
| 109 |          |     | B   |     |     | T   |
| 110 |          |     | A   |     |     | F   |
![[Screenshot_20211119_084031 1.png]]

1. Pretvorite vrednosti atributa D v primerih 200, 201 in 202 v KSP format (prestopno leto je odebeljeno)! Rezultat zaokrožite na tri decimalna mesta! (10 točk)  
  
2. Skicirajte box-plot za vrednosti atributa G (upoštevajte le primere z zaporedno številko med vključno  
100 ter vključno 110)! (10 točk)  
  
3. Diskretizirajte atribut G na 4 enako visoke intervale (upoštevajte le primere z zaporedno številko med  
vključno 100 ter vključno 110)! Nov atribut G_d naj ima vrednosti G1, G2, G3 in G4. Skicirajte  
histogram! (10 točk)  
  
4. Uporabite algoritem OneR za klasifikacijo primerov s poznanim razredom! Upoštevajte le atribut E.  
Skicirajte (eno-nivojsko) odločitveno drevo! Kolikšna je napaka tega klasifikatorja?  
(15 točk)  
  
5. Uporabite algoritem Naivni Bayes za klasifikacijo primerov z neznanim razredom! Upoštevajte le  
atributa E in F. Pri izračunu verjetnosti uporabite Laplace-ovo oceno! (25 točk)  
  
6. Zgradite prvi nivo odločitvenega drevesa (korensko vozlišče) po metodi TDIDT (algoritem ID3) pri  
čemer upoštevajte le atribute E, F in G_d. Kot mero za »čistost« podmnožic uporabite informacijski  
prispevek (information gain). Tako dobljeno »delno« odločitveno drevo narišite ter ga uporabite za  
klasifikacijo primerov z neznanim razredom!