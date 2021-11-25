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
	