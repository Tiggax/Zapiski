## NALOGA
imamo ključe med  neki {0,1}
$x_1$=1111110
$x_2$=0001010110
$x_3$=0110000
$x_4$=011110

```mermaid
graph TB;
A[1]-- 0 ---B
B[2]-- 0 ---C[x2]
A-- 1 ---D
D-- 0 ---H
H-- 1 ---M
D-- 1 ---I
B-- 1 ---E
E-- 0 ---F
E-- 1 ---G
G-- 0 ---J
G-- 1 ---K

```
Stisnit po plasteh ->

```mermaid
graph TB;
subgraph ena
A 
end
subgraph dve
D
B
end
subgraph tri
C
E
H
I
end
subgraph stiri
F
G
M
end
A[1]-- 0 ---B
B[2]-- 0 ---C[x2]
A-- 1 ---D
D-- 0 ---H
H-- 1 ---M
D-- 1 ---I
B-- 1 ---E
E-- 0 ---F
E-- 1 ---G
G-- 0 ---J
G-- 1 ---K

```
vsak nivo je en $2^2$