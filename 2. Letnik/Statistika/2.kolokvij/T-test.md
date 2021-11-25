preizkušanje domnev o $\mu$ kadar $\sigma$ ni poznan

Če standardni odklon ni znan, potem σ nadomestimo z njegovo oceno, $s$. Kvantile standardne normalne porazdelitve nadomestimo s kvantili ene od t.i. Studentovih porazdelitev. **Studentove porazdelitve** so družina porazdelitev, ki se razlikujejo glede na število **prostostnih stopenj df** (angl. degrees of freedom). 
Če je n velikost vzorca, je: $$df=n-1$$
![[Screenshot_20211125_091030.png]]

Testna statistika je sedaj: $$T=\frac{\overline x-\mu^*}{\frac{s}{\sqrt n}}$$

Naj bo $t_p (df)$ p-kvantil Studentove porazdelitve pri stopnji prostosti $df$ .  
Pri stopnji značilnosti α ničelno hipotezo $H_0 : μ = μ^∗$ zavrnemo  
- v korist alternativne hipoteze 
	$H_1^+ : μ > μ^∗$ kadar $T > t_{1−α}(df)$  
- v korist alternativne hipoteze 
	$H_1^- : μ < μ^∗$ kadar $T < −t_{1−α}(df )$  
- v korist alternativne hipoteze 
	$H_1 : μ ,μ∗$ kadar $|T |> t_{\frac{1−α}{2}}(df)$
	
	Prag zavrnitve razberemo iz tabele (Table of critical values for Student's t distributions)
	
	če so vzorci veliki (recimo n>50), potem t-test da praktično enake p-vrednosti kot z-test
	
```ad-note
collapse: T
title: Primer:
	
Višina štiriletnih deklic je normalno porazdeljena s pričakovano vrednostjo μ in standardnim odklonom σ = 5 cm. Naključno izbran vzorec devetih deklic nam da višine:

| 101 | 91  | 93  | 103 | 91  | 101 | 103 | 95  | 95  | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- |	

Pri stopni značilnosti $\alpha=0.1$ testirajmo ničelno hipotezo
$H_0:\mu = 100cm$

od zadnjič vemo:
- $\overline x =97cm$
- $s =5cm$
- testna statistika je: $t=-1.8$ (glej [[Intervalsko ocenjevanje in testiranje statističnih domnev#^328325]])

- stopnja prostosti je $df=n-1=8$

---

- $H_1 : μ\ne 100$  
	Iz tabele razberemo prag zavrnitve t0.95 = 1.86. H0 torej ne zavrnemo v korist $H_1$ (odstopanja niso statistično značilna).  
- $H_1^- : μ < 100$  
	Prag zavrnitve je sedaj −t0.9 = −1.397. H0 torej zavrnemo v korist $H_1$ (odstopanja so statistično značilna)
	

## Ali se zadnji sklep spremeni, če α = 0.05?
Za:
- $H_1^- :\mu < 100$
- $\alpha =0.05$
razberemo prag zavrnitve $-t_{0.95}=-1.86$. V tem primeru odstopanja niso statistično značilna.
```

---

**IZ**  za $\mu$ pri dani stopnju zaupanja $0<\beta<1$ je sedaj:
$$(\mu_{min},\mu_{max})=(\overline x -\frac{s}{\sqrt n}t_{\frac{1+\beta}{2}}\ ,\ \overline x +\frac{s}{\sqrt n}t_{\frac{1+\beta}{2}})$$

```ad-note
collapse: T
title:Primer:
## Za prejšni primer je za $\beta=0.95$
$\mu_{min}=93.9$
$\mu_{max}=100.1$

torej je 95% interval zaupanja za $\mu$ interval $(93.9,100.1)$ 
```
## Primerjava povprečij dveh spremenljivk na istih enotah
#TODO
Denimo, da na eni populaciji preu ˇcujemo dve intervalski spremenljivki, X  
in Y. Naj bo μX pri ˇcakovana vrednost prve, μY pa pri ˇcakovana vrednost  
druge spremenljivke v celotni populaciji.  
Testiramo ni ˇcelno hipotezo  
H0 : μX = μy  
proti eni od alternativnih hipotez: dvostranski (H1 : μX ,μy ), enostranski  
v korist X (H+  
1 : μX > μy ) ali enostranski v korist Y (H−1 : μX < μy ).  
Test enakosti povpre ˇcij se v tem primeru prevede na Z- ali t- test za  
spremenljivko X −Y .
(glej Statistika P716/18)

```ad-note
collapse: T
title: Primer:
Rezultati obeh kolokvijev Statistike za skupino sedmih študentov so dani v naslednji tabel:

| 1.Kolokvij(X) | 2.Kolokvij(Y) | D=X-Y |
| ------------- | ------------- | ----- |
| 72            | 57            | 15    |
| 61            | 47            | 14    |
| 52            | 71            | -19   |
| 48            | 52            | -4    |
| 92            | 77            | 15    |
| 69            | 81            | -12   |
| 56            | 49            | 7     | 

Pri stopnji značilnosti α = 0.05 testirajmo ničelno hipotezo, da je povprečje točk na 1. kolokviju enako kot povprečje točk na 2. kolokviju.

---

$H_0:\mu_x-\mu_y=0$
$H_1:\mu_x-\mu_y\ne0$
Testna statistika je:
$t=\frac{(\overline x-\overline)}{}$

```