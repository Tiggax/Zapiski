[[pearson.png|**Pearsonov**]] koficient korelacije
[[spearman.png|**Spearmanov**]] koficient korelacije

# Pearsonov
par slučajnih spremenljivk $(X,Y)$, ki je porazdeljen po **dvorasežni normalni porazdelitivi** $$N(\mu_x,\mu_y,\sigma_x,\sigma_y,\rho)$$
ima funkcijo gostote:
![[Screenshot_20211223_092257.png]]

število $\rho$ je **koeficient korelacije**. zanj velja:
- $-1\le\rho\le1$
- $\rho(x,y)=\rho(y,x)$
- $\rho(x,x)=1$

## Pearsonov koeficient korelacije
$$r=\frac{\sum_{i=1}^nx_iy_i-n\overline x\overline y}{sqrt{(\sum_{i=1}^n x_j^2-n\overline x^2)(\sum_{i=1}^ny_i^2-n\overline y^2)}}$$
vrednost je med -1 in 1. če je r > 0 govorimo o **pozitivni** povezanosti spremenljivk, če je pa 
r < 0 pa govorimo o **negativni**.
![[Screenshot_20211223_093138.png]]
#TODO prd11/sljd6

# Spearmanov
temelji na šibkejši predpostavki o monotoni povezavi.

**Ideja:** podatke nadomestimo z njihovimi rangi, in izračunamo Pearsonov koficient korelacije na rangih.