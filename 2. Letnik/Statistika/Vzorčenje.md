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
$$\sigma ^2 = \frac{1}{n}\sum _{i=1}^n(X_i-\overline{X})^2$$
izkaže se da ta ocena ni nepristranska ($E(\hat{\sigma} ^2)\ne\sigma ^2$) velja:
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
>$$P()$$