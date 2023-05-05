$y = f(x)$
$dy = (\frac{dy}{dx})dx$ - is a messure of sensitivity
$k = \tan(\alpha)= \frac{dy}{dx}$

Functions of multiple variables

$z = f(x,y))$
$y = c \to z = f(x)$
$dz = \frac{\partial z}{\partial x}y\ dx$
$x = c \to z = f(y)$
$dz = \frac{\partial z}{\partial y}x\ dy\ \to$ sensitivity at a fixed $x$.

TOTALNI odvod...
$dz = \frac{\partial z}{\partial x}y\ dx + \frac{\partial z}{\partial y}x\ dy$


# Equation of state

State defines the conditions that our system is exposed to.
By defining only two of the listed variables, the state is uniqly defined.

$V = f(P,T)$ - **equation of state**

$dV = (\frac{\partial V}{\partial P})T\ dP + (\frac{\partial V}{\partial T})P\ dT$ - total differencial

## Isohorous
means constant volume.
$0=(\frac{\partial V}{\partial P})T\ dP + (\frac{\partial V}{\partial T})P\ dT$
$$
\begin{align}
0 &= (\frac{\partial V}{\partial P})T\ dP + (\frac{\partial V}{\partial T})P\ dT\\
0 &= \frac{\partial V}{\partial T}P + \frac{\partial V}{\partial P}T \frac{\partial V}{\partial T} V\\
\frac{\partial V}{\partial T}V\frac{\partial V}{\partial P}T &= -\frac{\partial V}{\partial T}P\\
\\
\frac{\partial P}{\partial T}V &= -\frac{\frac{\partial V}{\partial T}P}{\frac{\partial V}{\partial P}T}
\end{align}
$$


## Expansion coefficiant
$$\alpha = \frac{1}{V}\frac{\partial V}{\partial T}P\ [K^{-1}]$$
## Tension coeffician
$$\beta = \frac{1}{P}\frac{\partial P}{\partial T}V\ [K^{-1}]$$
## Compressibility coeffician
$$\kappa = -\frac{1}{V}\frac{\partial V}{\partial P}T\ [bar^{-1}]$$

$\frac{\partial V}{\partial T}P = \alpha V$
$\frac{\partial P}{\partial T}V = \beta P$
$\frac{\partial V}{\partial P}T = \kappa V$


$\frac{\partial P}{\partial T}V = \beta P = \frac{\alpha}{\kappa}$

### Primer:
Joc is wants to skip the exam, so he pretends to be sick. He overheats the $Hg$ thermometer, which measures $T$ till 50°C, to 51°C the thermometer explodes. Why?

At 50°C the Volume is constant , as well as T increases P.

From Graph:
- $\kappa=39*10^{-12}$
- $\alpha = 18*10^{-5}$

Preassure will not build up immensly so we read out at 0.
$$(\frac{\partial P}{\partial T})V = \frac{\alpha}{\kappa} = \frac{18*10^{-5}}{39*10^{-12}}[\frac{bar}{K}]$$
$$=\$$
