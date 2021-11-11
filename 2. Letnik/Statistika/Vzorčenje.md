# Splošno
je način pridobivanja informacij o (načeloma veliki) populaciji s preučevanjem dela populacije.
N.p.r:
- javnomnenske ankete pred volitvami

# Točkasto ocenjevanje parametrov
recmo d aje celotna populacija velikosti $N$
želimo oceniti:
- populacijsko povprečje(aritmetična srredina)
	>$$\mu = \frac{x_1+x_2+...+x_n}{N}$$

- vsota
>$$\tau	= \sum_{i=1}^N x_i$$

- populacijska varianca


naključno vzorčenje je nepristransko.

## Vzorčna porazdelitev
porazdelitev $\overline{X}$ 

varianca vzorčne porazdelitve
>$$Var(\overline{X})=\frac{\sigma ^2}{n}(1-\frac{n-1}{N-1})$$
>faktor $\frac{n-1}{N-1}$ je **popravek končne populacije**, če je n<<N, pa lahko popravek zanemarimo:
>$$Var(\overline{X})\approx \frac{\sigma ^2}{n}$$

### Populacijska varianca
($E(\hat{\sigma} ^2)\ne\sigma ^2$) velja:
>$$E(\hat{\sigma} ^2)=\sigma ^2 \frac{N}{N-1}\frac{n-1}{n}$$
>ker je $\frac{N}{N-1}\frac{n-1}{n}<1$ varianco vedno **podcenimo**

### Nepristranska ocena variance
za manjše populacije:
>$$s^2=\frac{N-1}{N}\frac{1}{n-1}\sum _{i=1}^n(X_i-\overline{X})^2$$

za večje pa:
>$$s^2=\frac{1}{n-1}\sum _{i=1}^n(X_i-\overline{X})^2$$

za vzorčne porazdeltvne:
>$$Var(\overline{X})=S_{\overline{X}}^2=\frac{s^2}{n}(1-\frac{n}{N})$$

### Centralni limitni izrek
z $\overline{X}_n$ označimo vzorčno porazdelitev, če so vzorci velikosti n. Če F označuje  porazdelitvno funkcijo standardne normalne slučajne spremenljivke N(0,1) potem izrek pove:
>$$P(\frac{\overline{X}_n-\mu}{\frac{\sigma}{\sqrt{n}}}\ge z)\to F(z)$$

```ad-note
collapse: T
title: Primer:

Denimo da je višina v populaciji štirihletnih deklic normalno porazdeljena z $\mu =100cm$ in $\sigma =4cm$. iz populacije smo izbrali devet štiriletnih deklic, in jim izmerlili višino in dobili $\overline{x}=97cm$
- kako tipičen je ta vzorec t.j. kakšen delež vseh velikosti n=9 ima povpreče vsaj 97cm?

>$$P(\overline{X}\le 97)=P(\frac{\overline{X}-100}{\frac{4}{3}}\ge \frac{97-100}{\frac{4}{3}})=P(Z\ge -\frac{9}{4})=1-P(Z< -\frac{9}{4})=1-0.0122=0.9878$$

Torej približno 98.8% vzorcev velikosti 9 ima povprečje vsaj 97 cm.

- kakšen delež aritmetičnih sredin vseh vzorcev velikosti n = 9 se od poulacijskega povprečja razlikuje za vsaj 3 cm.
> A: 0.0244
>približno 2.4%v vzorcev velikosti 9.

- kako velik naj bodo vzorci, da bo delež vzorcev, katerih sredina se bo od populacijskega povprečja razlikovala največ 2 cm večji od 90 %?
>iščemo:
>$$P(|\overline{X}-100|\le 2)=0.9$$
>potem bo za vsak m$\ge$n:
>$$P(|\overline{X}-100|\le 2)\ge 0.9$$
>$$$$


```