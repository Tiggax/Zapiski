## Indeksi s stalno osnovo

^209cef

$X$ je številska slučajna spremenljivka in $x_i$ vrednosti te spremenljivke v i-ti skupini (i=1,...,K)
Zaporedje:
$x_1,x_2,x_3,...,x_k$  imenujemo <span style="color:red">statična vrsta</span>
če izberemo en podatek v vrsti in ga označimo $x_0$. to število imenujemo <span style="color:red">stalna osnova</span>.
indekse z osnovo $x_0$ izračunamo:
>$I_{i/0}=100*\frac{x_i}{x_0}; i=1,...,K$

Za izračun mora biti merska lestvica spremenljivke razmernostna,vrednosti pa pozitivne.
```ad-note
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
izraža upad ali prirast v primerjavi s prejšnim obdobjem. 
>$S_{t/t-1}=100*\frac{x_t-x_{t-1}}{x_{t-1}}$
>ali
>$S_{t/t-1}=I_{t/t-1}-100\%$

```ad-example
collapse: T
title: Primer:
| Leto | Čebula | $Indeksi_{(osnova = 2010)}$ | Verižni indeksi | Stopnja rasti |
| ---- | ------ | --------------------------- | --------------- | ------------- |
| 2010 | 4667   | 100                         | -               | -             | 
| 2011 | 6333   | 135.70                      | 135.70          | 35.70         |
| 2012 | 5869   | 125.76                      | 92.67           | -7.33         |
| 2013 | 6074   | 130.15                      | 103.49          | 3.49          |
| 2014 | 7563   | 162.05                      | 124.51          | 24.51         |
| 2015 | 7286   | 156.12                      | 96.34           | -3.66         |
| 2016 | 10885  | 233.23                      | 149.40          | 49.40         |
| 2017 | 9709   | 208.04                      | 89.20           | -10.8         |
| 2018 | 9612   | 205.96                      | 99.00           | -1.00         |
| 2019 | 10101  | 216.43                      | 105.09          | 5.09          |
| 2020 | 12042  | 258.02                      | 119.22          | 19.22         |

```

```chart
type: line
labels: [2010,2011,2012,2013,2014,2015,2016,2017,2018,2019,2020]
series:
  - title: $Indeksi_{(osnova = 2010)}$
    data: [100,135.70,125.76,130.15,162.05,156.12,233.23,208.04,205.96,216.43,258.02]
  - title: Verižni indeksi
    data: [-,135.70,92.67,103.49,124.51,96.34,149.40,89.20,99.00,105.09,119.22]
  - title: Stopnja rasti
    data: [-,35.70,-7.33,3.49,24.51,-3.66,49.40,-10.8,-1.00,5.09,19.22]
width: 80%
beginAtZero: true
```