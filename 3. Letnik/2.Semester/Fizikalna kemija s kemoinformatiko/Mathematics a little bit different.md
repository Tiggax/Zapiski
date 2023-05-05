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
$$(\frac{\partial P}{\partial T})V = \frac{\alpha}{\kappa} = \frac{18*10^{-5}}{39*10^{-12}}[\frac{Ps}{K}]$$
$$=46.1 [\frac{bar}{K}]$$
So now we know, that the thermometer is normaly at 1 bar, if we change the temperature by 1K, we get:
$$\begin{align}
(\frac{\partial P}{1})V &= 46.1 [\frac{bar}{K}]\\
\partial P &= 46.1 [bar]
\end{align}$$
so, that means, that the Pressure changes in the thermometer by 46.1 bars for each degree of Kelvin.

# Gas phase
low pressure - till 1 $atm$

## Boyle law
- $T$ is constant
- $PV$ is constant

![Hyperbolic inverse ^hypbl ](https://dr282zn36sxxg.cloudfront.net/datastreams/f-d%3A83808d2f02b11ce819e8b2dff89f9719eb7ec1d67b541addd38201d5%2BIMAGE_THUMB_POSTCARD_TINY%2BIMAGE_THUMB_POSTCARD_TINY.1) ^b798a8

The $P$ and $V$ are inverse porportional
## Guy-Lussac
- $P = C$ 
- $\frac{V}{T} = C$
![ ^gay-lussac ](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn1.byjus.com%2Fwp-content%2Fuploads%2F2019%2F08%2FGay-Lussacs-law.png&f=1&nofb=1&ipt=3a65d25ea9777f3893c8fb9ce1e80c3402d2832ff21789aebedf929d6268ffb0&ipo=images)

$Def:$ **Ideal Gas** is a hypothetical gas which follows both laws at all conditions (at immmediate and high pressures) ^ideal-gas


$$\begin{align}
V &= f(P,T)\\
dV &= (\frac{\partial V}{\partial T})P\ dT + (\frac{\partial V}{\partial P})T\ dP\\
\end{align}$$
 and we know that Gay-Lussac: $(\frac{\partial V}{\partial T})P = C = \frac{V}{T}$, and
 Boyle law: $(\frac{\partial V}{\partial P})T = C = -\frac{V}{P}$
 
 $$\begin{align}
 dV &= \frac{V}{T}\ dT - \frac{V}{P}\ dP\\
 \frac{dV}{V} &= \frac{dT}{T} - \frac{dP}{P}
 \end{align}$$
by: $\frac{1}{x}dx= ln(x)$
$$\ln(V) = \ln(T) - \ln(P)$$
$$\begin{align}
d(\ln(V)) &= d(\ln(T)) - d(\ln(P))\\
d(\ln(V)) - d(\ln(T)) + d(\ln(P))&= 0\\
d(\ln(V) - \ln(T) + \ln(P)) &= 0\\
\ln\left(\frac{PV}{T}\right)= C
\end{align}$$

What we get is that the hyperbolas in [[#^b798a8|graph]] are of different temperatures.
and  the lines in [[#^gay-lussac]]
