## Indeksi s stalno osnovo

^209cef

$X$ je številska slučajna spremenljivka in $x_i$ vrednosti te spremenljivke v i-ti skupini (i=1,...,K)
Zaporedje:
$x_1,x_2,x_3,...,x_k$  imenujemo <span style="color:red">statična vrsta</span>
če izberemo en podatek v vrsti in ga označimo $x_0$. to število imenujemo <span style="color:red">stalna osnova</span>.
indekse z osnovo $x_0$ izračunamo:
>$I_{i/0}=100*\frac{x_i}{x_0}; i=1,...,K$

Za izračun mora biti merska lestvica spremenljivke razmernostna,vrednosti pa pozitivne.
```ad-example
collapse: T
title: Primer:

| Dežela   | število nasadov | $indeks_{[Primoje]}$ |
| -------- | --------------- | -------------------- |
| Podravje | 17769           | 126.77               |
| Posavje  | 15292           | 109.1                |
| Primorje | 14017           | 100                  |
| IVD      | 246             | 1.76                 | 
```
### časovna vrsta
ko se  $X$ spreminja v času, jo imenujemo <span style="color:red">časovna vrsa</span>, število $T$ pa dolžina statične vrste.
## Verižni indeksi
delujejo kot  [[#^209cef|indeksi s stalno osnovo]],a za osnovo uzamemo  predhodnji podatek.
>$I_{t/t-1}=100*\frac{x_t}{x_{t-1}}; t=2,...,T$

ker prvi podatek nima predhodnika, prvi verižni indeks ne obstaja. verižni indeksi so smiselni le, če je časovna vrsta ekvidistančna.

## Stopnja rasti