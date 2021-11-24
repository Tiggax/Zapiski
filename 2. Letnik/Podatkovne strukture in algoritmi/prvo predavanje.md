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
### Razpršilna funkcija

![[Screenshot_20211124_131850.png]]

če so ključi k naključna realna števila enakomerno prazdeljena na intervalu $[0,1)$. potem funkcija: $$h(k)=k*m$$ zadošča zgornjem pogoju. *funkcija razpršuje*

### Zgoščevalna funkcija
#### deljenje

kaj nardimo če je k Celo število?
če je celo število rešimo z Modulom velikosti tabele.** ta funkcija deluje po metodi deljenja.**
primer:
1769 mod 256= 11 bitov
$$h(k)=k*mod\ m$$
če sta si števili tuji, potem vsi

če je m dovolj veliko praštevilo, je tuje glede na k

Primer:
2000 ključev, je za dolžina 3

#### množenje
$$h(k)= (k*p)\ mod\ m$$
kjer je $p$ neka konstanta.
- vrednost m ni kritična

lahko jo zapišemo tudi kot: $$h(k)=m(kA\ mod\ 1)$$; kjer je 0<A<1 in x mod 1 pomeni dec del x. v tem primeru je Knuth A$\approx\frac{(\sqrt{5} -1)}{2}=0.6180339887...$

#### naslavljanje
ko pride đorđe na avtobus more pregledat vse stole da so prazni. drugače bi mislil da je avtobus poln in čaka naslednjega. hočemo najti čim prej najti prosto mesto.

zgoščevalna funkcija ne slika več iz U v S 
sedaj slika: $$h:U\times \{0,1,...,m-1\} \to \{0,1,...,m-1\}$$

kaj pa če je tabela polna?

**deamortizacija** z neko konstanto prestavljaš elemente iz ene tabele v drugo v korakih skozi čas. s tem prišparaš na delu.


##### Linearno naslavljanje
če x ni na voljo-> preverim naslednjega -> preverim naslednjega ...
**Dobro:**
- Đorđe lahko najde sedež(lahko vstavljanje)

**Slabo**
- če je polje $i$ prazno, potem je verjetnost da ključ pride v $i+1$ enako $\frac{1}{n}$
- če je polje $i$ polno, potem je verjetnost da ključ pride v $i+1$ enako $\frac{(1+i)}{n}$

##### Kvadratično naslavljanje