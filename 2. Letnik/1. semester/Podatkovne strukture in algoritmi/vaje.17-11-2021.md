# Implementacija slovarja
## b drevesa
za razliko od dvojiških imajo vozlišča lahko več ključev, razedlimo pa lahko na k+1 podrazredov. Ključi so urejeni, med dvema ključema pa velja strogo večje ali manjjše. ker so vsi listi na istem nivoju, se lahko uravnotežijo.

rastejo "od spodaj navzgor"

### Primer:
v b drevo reda 5(=b) vstavi naslednje elemente(ključe)
20, 40, 10, 30, 15, 35, 7, 26, 18, 22, 5, 42, 13, 46, 27, 8, 32, 24, 45, 25
```mermaid
graph LR
A[10,20,30,40]
```
ker je reda 5 je so notri največ 4 elementi. nasednji element se vstavi naprej
```mermaid
graph TB
A[20]
B[10,15]
A---B
C[30,40]
A---C
```
vstavimo naslednje: 35, 7, 26, 18
```mermaid
graph TB
A[20]
B[7,10,15,18]
A---B
C[26,30,35,40]
A---C
```
Vstavimo 22:
```mermaid
graph TB
A[20,30]
B[7,10,15,18]
A---B
C[22,26]
A---C
D[35,40]
A---D
```
Vstavimo: 5
```mermaid
graph TB
A[10,20,30]
A---B[5,7]
A---B1[15,18]
A---C[22,26]
A---D[35,40]
```
Vstavimo: 13, 46, 27, 8, 32
```mermaid
graph TB
A[10,20,30]
A---B[5,7,8]
A---B1[13,15,18]
A---C[22,26,27]
A---D[32,35,40,46]
```
Vstavimo: 42
```mermaid
graph TB
A[10,20,30,40]
A---B[5,7,8]
A---B1[13,15,18]
A---C[22,26,27]
A---D[32,35]
A---D1[42,46]
```
Vstavimo: 24, 45
```mermaid
graph TB
A[10,20,30,40]
A---B[5,7,8]
A---B1[13,15,18]
A---C[22,24,26,27]
A---D[32,35]
A---D1[42,45,46]
```
Vstavimo 25:
```mermaid
graph TB
E[25]
E---A[10,20]
E---A1[30,40]
A---B[5,7,8]
A---B1[13,15,18]
A---C[22,24]
A1---C1[26,27]
A1---D[32,35]
A1---D1[42,45,46]
```
koliko je višina: $\log_n$(če je b konstanta)
**Brisanje:** 25
minimalno število je:2 ker je reda 5. ko zbrisemo naredimo podobno kot pri binarnem:
brišemo x in nadomestimo z max(levega) ali pa min(desnega)
ker so v nekaterih reda 1(<2) se jih prestavi gor, in preuredi drevo.
```mermaid
graph TB
A[10,20,26,40]
A---B[5,7,8]
A---B1[13,15,18]
A---C[22,24]
A---D[27,30,32,35]
A---D1[42,45,46]
```
**Brisanje:** 45, 24, 32
```mermaid
graph TB
A[10,20,27,40]
A---B[5,7,8]
A---B1[13,15,18]
A---C[22,26]
A---D[30,35]
A---D1[42,46]
```
#### Primer: B drevo reda 4
v b drevesu reda 4 vstavimo naslednje elemente: 22,11,6,13,17,27,8,15,1
največ: 3 ključi
najman: 1 ključ
```mermaid
graph TD
A[5, 11, 17]
A---B[1]
A---B1[6,8]
A---C[13,15]
A---D[22,27]
classDef red fill:#f34
```
če ima en ključ je: list ali koren
če ima dva ključa:
če ima tri ključe: 
```mermaid
graph TD
A[11]
A---B[5]
A---B1[17]
B---C[1]
B---C1[8]
B1---C2[15]
B1---C3[27]
C---X1
C---X2
C1---D[6]
C1---X3
C2---D1[13]
C2---X4
C3---D2[22]
C3---X5
D---X6
D---X7
D1---X8
D1---X9
D2---X10
D2---X11
classDef red fill:#f34
```

#### Primer: B drevo
vstavimo elemente v B-drevo rda 4 in Č-R drevo
## Rdeče-črna drevesa
ekvivalentna 2,3,4 drevesom. so binarna. iskalna (levo<x<desno), imajo še poleg ključa barvo vozlišča (0,1). če pogledate katerokoli pot od vozlišča do lista bo št. črnih in št rdečih enaka. uravnotežena v smislu črno-rdeče. koren je vedno **Črn**, listi so vedno **črni in brez informacij.** vsakemu rdečemu vozlišču mora slediti črno.

#### Primer: B drevo
vstavimo elemente v B-drevo rda 4 in Č-R drevo
elemente: 4,7,12,15,3,5,14
prvi element vstavimo kot črno, drugače kot rdeče.
```mermaid
graph TD
A[4č]
A---X1
A---B[7r]
B---X2
B---C[12r]
C---X3
C---X4
```
nardimo rotacijo
```mermaid
graph TD
A[7č]
A---B[4r]
A---B1[12r]
B---X2
B1---X3
B1---C[15r]
C---X4
C---X5
```
Prebarvamo:
```mermaid
graph TD
A[7č]
A---B[4č]
A---B1[12č]
B---X2
B---X3
B1---X4
B1---C[15r]
C---X5
C---X6
classDef red fill:#f34
```
Vstavimo 3,
```mermaid
graph TD
A[7č]
A---B[4č]
A---B1[12č]
B---C[3r]
B---X3
B1---X4
B1---C1[15r]
C1---X5
C1---X6
classDef red fill:#f34
```
Vstavimo 5;
```mermaid
graph TD
A[7č]
A---B[4č]
A---B1[12č]
B---C[3r]
B---C1[5r]
B1---X4
B1---C2[15r]
C1---X5
C1---X6
C2---X7
C2---X8
classDef red fill:#f34
```
Vstavimo 14
```mermaid
graph TD
A[7č]
A---B[4č]
A---B1[12č]
B---C[3r]
B---C1[5r]
B1---X4
B1---C2[15r]
C1---X5
C1---X6
C2---D[14r]
C2---X8
D---X9
D---X10
classDef red fill:#f34
```
obrnemo:
```mermaid
graph TD
A[7č]
A---B[4č]
A---B1[14č]
B---C[3r]
B---C1[5r]
B1---C2[12r]
B1---C3[15r]
C1---X5
C1---X6
C2---X8
C2---X7
C3---X11
C3---X12
classDef red fill:#f34
```