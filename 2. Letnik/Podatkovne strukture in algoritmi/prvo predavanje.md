# slovarji
- linearno drevo
- binarno
- B drevo
---
- neskončni seznam (vklučuje random vrednosti)


| kakšen?                              | čas | T           | P           | S    |
| ------------------------------------ | --- | ----------- | ----------- | ---- |
| linearno drevo<br>binarno<br>B drevo |     | $O(\log_n)$ |             | O(n) |
| neskončni seznam                     |     | $O(\log_n)$ | naključnost | O(n) |
| razp tabela                          |     | O(1)        | -//-        | O(n) | 



## razpršena tabela
ključi bodo it univerzalne množice $Z$ (omejena na Bite -> 32 bitna je $32^2$)

tabela veliksti U ima U bitov
- vstavljamo tako da 1 je v 0 ni v slovarju.
- tabela je velika sorazmerno z univerzalno množico.
- uporabimo naključnost?
- velikost bo v odvisnosti od n elementov
- izvedejo se v konstantnem času
	- S zmanjšamo na 

- dodamo razpršilno funkcijo $S(H(x))$-> H razprši neki neki...
- zgoščevalno funkcijo ...

![[Screenshot_20211124_123336.png]]

funkcija h je določena v naprej -> neizpodbitno obsojena na samo injektivnost, ker slika iz večje v manjšo bo zih slikala dva ključa v isti element![[Screenshot_20211124_124131.png]]
ta problem moramo rešiti:
kako rešiti problem sovpadanja?
neka anologija z avtobusom pa sedeži
se nekam hoče zint, če je zaseden gre na naslednje mesto, in ponavlja...
ta način je linearen (največ n-krat ponovitev)
tu nas bo rešila naključnost

Temu se reče **naslavljanje**

### veriženje
dodaš pomožne node ali "stolčke", kjer dobimo na koncu največ n- pomožnih "stolčkov"
je podobno linearna za(največ k-krat; k=št stolčkov)
#neurejen-seznam 

veriženje ali "chaining" je veriženje novega slovarja. je postopek pri katerem rešujemo soupadanje z novim seznamom, v katerega vstavimo elemente, ki sovpadajo s tem elementom. 
![[Screenshot_20211124_125259.png]]

v najslabšem primeru $\theta(n)$
do pričakovane pridemo z upoštevanjem naključnosti. 

primer golobnjaka:
mečemo fnikulo v predalčke
P(1)=$\frac{1}{n}$
P(2)=$\frac{1}{n}$
			...
če je metanje frnikule naključno je verjetnost da pade v vsakega $\frac{1}{n}$
kakšna je vrjetnost da jih 5 pade v isti predal?

s tem zagotovimo da bo v $\frac{1}{n^k}$


$|U|=$-m- M
$|S|=m=c*n$

