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
# Spearmanov
temelji na šibkejši predpostavki o monotoni povezavi.

**Ideja:** podatke nadomestimo z njihovimi rangi, in izračunamo Pearsonov koficient korelacije na rangih.