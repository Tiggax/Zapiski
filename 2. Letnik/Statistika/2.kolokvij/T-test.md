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
```