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
prav tako:
