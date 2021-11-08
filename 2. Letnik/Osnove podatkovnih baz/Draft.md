## Zahteva po strani
- če iskana dtran ni v bazenu:
	- izberi okvir za **zamenjavo**
	- če je okvir "umazan" potem se mora zapisati na Disk
	- Preberi izbrano stran v izbrani okvir
- **pripni** strani in vrni njen naslov
---
## Več o delu
- zahtevana stran mora biti *odpeta*
- vidno mora biti če je stran spremenjena ali "umazana"
	- umazan bit
- stran v bazenu je lahko zahtevana večkrat
	- uporablja se **število pripenjanj**.  Stran je kandidat za zamenjavo če je št. pripenjanj =0
- vzporednost in okrevanje:
	- dodatni I/O v primeru da je stran izbrana za zamenjavo
- protokol dnevnika
---
## Strategije za zamenjavo strani
- okvir izbran s **strategijo zanenjave**
	- LRU, Ura(Clock), MRU, itd.
- Strategija ima lahko velik vpliv na # I/O operacij; odvisno od **vzorca dostopa**
- **Sekvenčno prelivanje:**
	- Grda situacija povzročena z LRU + ponavljajoč sekvenčni pregled tabele
	- **# okvirjev < # strani datoteke** vsaka zahteva povzroči I/O. MRU je v tem primeru boljša(toda ne v vseh situacijah)
---
## Format zapisa
```mermaid
graph LR;
	A--B
```