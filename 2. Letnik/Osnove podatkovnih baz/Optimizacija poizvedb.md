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


## Drevo operacij RA (brez algoritmov)
![[Screenshot_20211129_084025.png]]
