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

kaj vzamemo v alteranativno domnevo?
- najprej testiramo proti dvostranski domnevi:
$H_1:\mu$
```
