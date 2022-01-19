# 2
| spol/dodatek | gorčica | kečap | majoneza |
| ------------ | ------- | ----- | -------- |
| Z            | 15      | 23    | 10       |
| m            | 25      | 19    | 8        |
|              | 40      | 42    | 8        | 

$H_0:$spol in izbita nista povezani
$H_1:$ -//- sta povezani

$f_{11}'=\frac{48*40}{100}$

| spol/dodatek | gorčica | kečap | majoneza | skupaj |
| ------------ | ------- | ----- | -------- | ------ |
| Z            | 19.2    | 20.16 | 8.6      | 48     |
| m            | 20.8    | 21.84 | 9.36     | 52     |
|              | 40      | 42    | 8        | 100    | 

$$\chi^2=\sum_{i=1}^2\sum_{j=1}^3\frac{(f_{ij}-f_{ij}')^2}{f_{ij}}$$
= 2.95

stopnja prrostosti:
$\chi_{0.9}^2(2)=4.61$
ker je večja kot testna => $H_0$ obdržimo

# 3
| S(enol)x1 | S(dvolet)x2 | D$=\mu_{x2}-\mu_{x1}$ |
| --------- | ----------- | --------------------- |
| 16.3      | 16.5        | 0.2                   |
| 25.4      | 25.5        | 0.1                   |
| 10.6      | 10.7        | 0.1                   |
| 30.1      | 33.7        |                       |
| 11.8      | 14.7        |                       |
| 12.5      | 13.6        |                       |
| 20.6      | 21.5        |                       |

$H_0:$ $\mu_{x2}-\mu_{x1}=1$
$H_1:$$\mu_{x2}-\mu_{x1}\ne1$


testna statistika :
$$t=\frac{\overline d-\mu_0}{\frac{s_0}{\sqrt n}}$$

$$s_D^2=2.02$$
$t=0.5$
stopnja prostosti: n-1=6
iz tabele:
$t_{0.975}(6)=2.447$
ker pade v interval $(-2.447,2.447)$ => $H_{0}$ obdržimo

# 4

| izvedbe | prof(x) | student(y) | 
| ------- | ------- | ---------- |
| 1       | 2       | 4          |
| 2       | 6       | 1          |
| 3       | 3       | 3          |
| 4       | 8       | 5          |
| 5       | 4       | 8          |
| 6       | 7       | 6          |
| 7       | 5       | 2          |
| 8       | 1       | 7          |

$H_{0}:$ oceni prof in studenta nista povezani
$H_1:$ -//- sta povezani

spearmanov test
![[Screenshot_20220119_083152.png]]

$\overline x= 4.5$
$\overline y= 4.5$

$$\sum_{i=1}^8 x_iy_i=154$$
$$r_s=-0.19$$
pogledamo krit vrednost iz tabelce
n=8, $\alpha=0.05$ 
iz tabele: 0.738
ker je $|r_s|<0.738$ , $H_{0}$ obdrim.

# 5
| razpon  | $f_i$ |
| ------- | ----- |
| 180-189 | 9     |
| 190-199 | 11    |
| 200-209 | 14    |
| 210-219 | 10    |
| 220-229 | 6     | 

$H_{0}:$ $\mu_x=202cm$
$H_{1}:$ $\mu_x>202cm$

T-test
$t= \frac{\overline x-\mu_{x}}{\frac{s}{\sqrt n}}$

$\overline x= 203.1$
$s^2=163.3$
$t=0.61$
stopnja prostosti: n-1 = 49
$t_{0.95}(40)=1.684$
$t_{0.95}(60)=1.671$

