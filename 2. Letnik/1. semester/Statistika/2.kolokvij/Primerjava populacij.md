v dveh populacijah želimo analizirati statistično spremenljibko kot npr:
- uˇcinkovitost cepiva v dveh starostnih skupinah  
- koliˇcino padavin v dveh regijah  
- deleˇz kadilcev pri moˇskih in ˇzenskah  
- itd.

vzorec je lahko 
- **neodvisen**
- **odvisen**

# neodvisni vzorci
Naj bo X intervalska sluˇcajna spremenljivka, X1 naj oznaˇcuje X v 1.  
populaciji, X2 pa X v 2. populaciji.
če vemo standardni odklon dveh populacij, in je hkrati enak:
$$X_1\approx N(\mu_1,\sigma^2)\ \ \ \ \ X_2\approx N(\mu_2,\sigma^2) $$
če iz prve populacije izbiramo vzorce velikosti $n_1$, iz druge pa velikosti $n_2$ sta vzorčni porazdeltitvi: $$\overline X_1\approx N(\mu_1,\frac{\sigma^2}{n_1})\ \ \ \ \overline X_2\approx N(\mu_2,\frac{\sigma^2}{n_2})$$
 
če sta vzorca neodvisna velja:
$$\overline X_1 - \overline X_2 \approx N(\mu_1-\mu_2,\sigma^2(\frac{1}{n_1}+\frac{1}{n_2}))$$

>in torej:
>$$Z=\frac{(\overline X_1-\overline X_2)-(\mu_1-\mu_2)}{\sigma \sqrt{(\frac{1}{n_1}+\frac{1}{n_2})}}\approx N(0,1)$$

kadar populacijskih varianc ne poznamo, ju je potrebno	oceniti iz vzorcev:
>naj bodo $x_{1,1},x_{1,2},...,x_{1,n_1}$ vrednosti naključnega vzorca velikosti $n_1$ iz prve populacije in $\overline x_1$ vzorčno povprečje.
>**Nepristranska ocena za varianco** prve populacije je:
>$$s_1^2=\frac{1}{n_1-1}\sum_{j=1}^{n_1}(x_{1,j}-\overline x_1)^2$$
>podobno za drugo naredimo. 

če se vzorčni varianci ne razlikoujeta preveč, lahko domnevamo, da sta populacijski varianci enaki in vzorčni varianci zamenjamo z povprečno (skupno) varianco:
$$s_{skupna}^2=\frac{s_1^2+s_2^2}{2}$$
potem sledi:
$$T =\frac{(\overline X_1-\overline X_2)-(\mu_1-\mu_2)}{s_{skupni} \sqrt{(\frac{1}{n_1}+\frac{1}{n_2})}}$$
je studentova porazdelitev s stopnjami prostosti $$df= n_1+n_2-2$$

ne razlikujeta se preveč kadar konkretno:
$$\frac{max(s_1^2,s_2^2)}{min(s_1^2,s_2^2)}<2$$
če je večje od 2:
potem nista enaki in uporabimo studentovo porazdelitev:
>$$T=\frac{(\overline X_1-\overline X_2)-(\mu_1-\mu_2)}{ \sqrt{(\frac{s_1^2}{n_1}+\frac{s_2^2}{n_2})}}$$
>ki ima stopnjo prostosti:
>$$df=min(n_1 -1, n_2-1)$$

## Primerjava Bernulijevih verjetnosti
Sedaj ˇzelimo primerjati verjetnost nekega dogodka v dveh populacijah  
(t.j. vrednosti Bernoullijevih verjetnosti), npr.  
- verjetnost kalitve dveh sort  
- odstotek uˇcinkovitosti zdravila pri moˇskih in ˇzenskah  
- itd
![[Screenshot_20211209_091209.png]]
![[Screenshot_20211209_091236.png]]
![[Screenshot_20211209_091319.png]]
![[Screenshot_20211209_091350.png]]

# Odvisna vzorca
Pri neodvisnih vzorcih informacija prvega vzorca ni povezana z drugim  
vzorcem. Sedaj obravnavamo primer odvisnih vzorcev, ko je vsaka enota  
iz prve populacije v paru z enoto iz druge populacije.  
Npr.:  
- primerjamo znanje angleˇskega jezika ˇstudentov pred in po teˇcaju  
- primerjamo teˇzo pred in po dieti  
- itd.

![[Screenshot_20211209_094100.png]]
