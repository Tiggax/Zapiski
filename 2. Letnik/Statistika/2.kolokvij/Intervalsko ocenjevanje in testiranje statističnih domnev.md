# Z test
če poznamo standardni odklon vzorca, na podlagi naključnega vzorca, hočemo preizkusit domnevo, da je pop. povprečje za preučevano slučajno spremenljivko $\mu^2$
$$H_0 : \mu =\mu^*$$
**$H_0$** imenujemo **ničelna domneva**

pri $n$ je velikost vzorca in $\overline x$ povprečje naključnega vzorca. vrednost testne statistike je: $$Z=\frac{\overline X -\mu ^*}{\frac{\sigma}{\sqrt{n}}}$$
če $\overline x$ preveč odstopa od $\mu^*$(testna statistika se preveč oddali od 0)potem $H_0$ zavrnemo. preveč pomeni odvisno od:
- **alternativne hipoteze**
	![[Screenshot_20211125_084408.png]]
- **stopnje značilnosti** $\alpha$
	![[Screenshot_20211125_084504.png]]
	![[Screenshot_20211125_084620.png]]
	
```ad-note
collapse: T
title: Primer:
Višina štiriletnih deklic je normalno porazdeljena s pričakovano  
vrednostjo μ in standardnim odklonom σ = 5 cm. Naključno izbran  
vzorec devetih deklic nam da višine: 

| 101 | 91  | 93  | 103 | 91  | 101 | 103 | 95  | 95  | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- |

pri stopnji značilnosti $\alpha=0.05$ testirajmo hipotezo:
$H_0:\mu =100cm$

---

za ta vzorec dobimo $\overline x=97$, torej je statistika
$$Z=\frac{\overline X -\mu ^*}{\frac{\sigma}{\sqrt{n}}}=\frac{97-100}{\frac{5}{\sqrt{9}}}=-1.8$$

---

## kaj vzamemo v alteranativno domnevo?
- najprej testiramo proti dvostranski domnevi:
$H_1:\mu\ne 100cm$
Prag zavrnitve $H_0$ proti $H_1$ je $Z_{0.975} = 1.96$. Ker $|Z|< 1.96$, ničelne  
hipoteze ne zavrnemo. Rečemo, da odstopanja niso **statistično  
značilna**

---

## Ničelno domnevo sedaj testirajmo proti alternativni domnevi  
$H_1^+ : μ > 100 cm$.  
Testno statistiko moramo sedaj primerjati z vrednostjo $z_{0.95} = 1.65$,  
kar pomeni da $H_0$ seveda ne zavrnemo (odstopanja v desno ne  
morejo biti statistično značilna, če povprečje od ničelne hipoteze  
odstopa v levo).

#TODO 

Ni ˇcelno domnevo testirajmo ˇse proti alternativni domnevi  
H−1 : μ < 100 cm.  
Testno statistiko moramo sedaj primerjati z vrednostjo  
−z0.95 = −1.65, kar pomeni da H0 zavrnemo v korist alternativne  
hipoteze H−1 . Odstopanja so statisti ˇcno zna ˇcilna.  
⋄ Vzemimo sedaj α = 0.01 in ni ˇcelno domnevo testirajmo proti  
alternativni domnevi  
H−1 : μ < 100 cm.  
Testno statistiko moramo sedaj primerjati z vrednostjo  
−z0.99 = −2.33, kar pomeni da H0 ne moremo zavrniti v korist H−1 .
```

^328325

