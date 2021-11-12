# Odločitvena drevesa
- notranje vozišča predstavljajo atribut
- veja predstavlja rezultat tega testa n.p.r. "color =red"
- list predstavlja oznako razreda(ali porazdelitev vrednosti razreda)
- **v vsakem vozlišču**: en atribut je izbran, po katerem delimo učne primere v kar se da "čiste" podmnožice
- nove primere kasificiramo tako, da sledimo ustreznim potem v drevesu od korena do listov

## Gradnja drevesa
od zgoraj navzdol
- na začetku so vsi primeri v korenu drevesa
- rekurzivno delimo primere v podmnožicce s pomočjo atributov in  njihovih vrednosti.

## Rezanje drevesa
od spodaj navzgor
- odstranimo poddrevesa ali veje drevesa z namenom izboljšati točnost napovedi drevesa na novih primerih

## Izbor atributa za delitev primerov
- **v vsakem vozlišču drevesa:** ocenimo razpoložljive atribute glede na njihovo sposobonost delitve primerov na "čiste" podmnožice - uporabimo **funkcijo primernosti**(goodness function)
- Tipične funkcije:
	- Informacijski prispevek (ID3, C4.5) 
	- Raazmerje informacijskega prisp