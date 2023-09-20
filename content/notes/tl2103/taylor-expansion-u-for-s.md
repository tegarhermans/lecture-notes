---
title: "taylor expansion u(x) for s(u, x, E)"
date: 2023-09-19T19:34:00+07:00
authors: ['Sparisoma Viridi']
tags: ['TL2103']
draft: false
math: true
url: "0054"
---
{{< toc >}}


## place
Estuary is coastal water body where streams from rivers mixes with streams from the ocean.


## concentration
Concentration of single point source conservative pollutant in an estuary is as follow

$$\tag{1}
s = s_0 \exp \left( \frac{xu}{E} \right)
$$

for $x \le 0$,  where $s$ is final centration $\rm (mg/L)$, $u$ is velocity $\rm (miles/day)$,  $x$ is distance from point source $\rm (miles)$. There are coefficients for initial concentration $s_0 = 350 \ {\rm mg/L}$ and tide wave dispersion coefficients $E = 5 \ {\rm miles^2/day}$.


## velocity
In a certain estuary the velocity can be formulated as

$$\tag{2}
u(x) = | \sin 4.8x|.
$$


## task
+ Use Taylor series to approximate the value of velociy for given distance $u(x)$ until 5% error result.
+ Use the aproximation value of velocity to calculate the concentration pollutant in particular distance in the estuary $s(x)$


## output
+ If $x > 0$, repeat ask for $x$
+ $x = -1 \ {\rm miles}$
+ $N = 15$
+ $u = 0.98452 \ {\rm miles/day}$
+ $\epsilon = 1.1692 \ \\%$
+ $s = 287.4445 \ {\rm mg/L}$


## taylor series
In general a function $f(x)$ can be approximated to $N+1$ terms

$$\tag{3}
f(x) \approx \sum_{n=0}^N \frac{(x - x_0)^n}{n!} \left. \frac{d^n f(x)}{dx^n} \right|_{x=x_0} = \sum _{n=0}^N g_n(x), 
$$

which is known as Taylor series. And for $f(x)$ in Eqn (2) it would be similar to

$$\tag{4}
f(x) = \sin ax.
$$

### $n = 0$
$$\tag{5.0}
g_0(x) = \sin a x_0.
$$

### $n = 1$
$$\tag{5.1}
g_1(x) = (x - x_0) \cdot a \cos a x_0.
$$

### $n = 2$
$$\tag{5.2}
g_2(x) = \tfrac12(x - x_0)^2 \cdot -a^2 \sin a x_0.
$$

### $n = 3$
$$\tag{5.3}
g_3(x) = \tfrac16 (x - x_0)^3 \cdot -a^3 \cos a x_0.
$$


## general form
Eqns (5.0) - (5.3) can be represented in

$$\tag{6.0}
h_0(x) = g_0(x) + g_1(x)
$$

and

$$\tag{6.1}
h_1(x) = g_2(x) + g_3(x),
$$

or

$$\tag{7}
h_m(x) = g_{2m}(x) + g_{2m+1}(x)
$$

in general with $m = 0, 1, ..$.
