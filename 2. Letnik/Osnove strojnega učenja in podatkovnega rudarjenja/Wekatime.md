## Učenje enostavnih pravil
### 0R
|       | $A_1$ | $A_2$ | ... | $A_n$ | C   |
| ----- | ----- | ----- | --- | ----- | --- |
| $v_1$ |       |       | ... |       | X   |
| $v_2$ |       |       | ... |       | Y   |
| $v_3$ |       |       | ... |       | X   |
| ...   | ...   | ...   | ... | ...   | ... |
| $v_m$ |       |       | ... |       | X   |

ne upošteva podatkov v stolpcih($A_n$) ali vrstic ($v_n$) ampak po razredih (C)

### 1R
```mermaid
graph TD
A[Outdoor]
A-- s ---B[""{y,y,n,n,n}=NO"]
A-- n ---C[""{y,y,y,y,y}=YES"]
A-- r ---D[""{n,n,y,y,y}=YES"]
```