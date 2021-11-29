(Query optimization)
# Osnove
**Potek:**
- plan izvajanja
	- prevajanje SQL v RA
	- Ocenitvena funkcija
	- algoritmi za izvajanje operacij RA

**sistem R:**
- najbolj razširjen
- dela v redu < 15 stikov

## Program v SUPB
Kaj je program v SUPB?
- Drevo operacij relacijske algebre
- vozlišča so označena z algoritmi za izvajanje posamičnih operacij.
![[Screenshot_20211129_084234.png]]

Drevo iteratorjev:
- vsaka operacija je implementirana z  iteratorjem
- vmesniki iteratorja: open(), next(), close()
- klic operacije $X$ sproži evaluacijo operacije $X$ na otrocih
- na rezultatih otrok operacija izvaja svojo kodo
- rezultate pošilja staršem(zapis po zapis ali blok zapisov)

S tem dobim **drevesno strukturiran cevovod** po katerem se pretakajo n-terice
	- na nekaterih mestih pretok začasno ustavi zaradi materializacije tabel.
### Drevo operacij RA (brez algoritmov)
![[Screenshot_20211129_084025.png]]
### Drevo operacij RA (z izbranimi algoritmi)
![[Screenshot_20211129_084834.png]]

## Optimizacija drevesa operacij
kako?
**logična:**
**Fizična:**
## Prevajanje SQL v relacijsko algebro
Dekompozicija poizvedbe v bloke
- celoten SQL stavek se razdeli v bloke
- zaključeni SQL bloki se obravnavajo kot procedure
- **posledica:** vgnezdeni bloki se kličejo ob vsaki iteraciji v nadrejenem bloku.

## Ocena plana izvajanja
Rezultat je vedno približek!
Statistika shranjena v sistemskih katalogih
- za oceno hitrosti izvajanja plana izvedbe
- za oceno velikosti vmesnih rezultatov
Cene posameznih operacij smo si ogledali na  prejšnem predavanju
- sekvenčni pregled, indeksnu pregled, stuik z zanko, stik z indeksom, i.t.d.

Pri oceni se uporabi cena CPU in I/O