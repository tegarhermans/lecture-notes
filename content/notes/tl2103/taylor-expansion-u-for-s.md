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

$$
s = s_0 \exp \left( \frac{xu}{E} \right)
$$

for $x \le 0$,  where $s$ is final centration $\rm (mg/L)$, $u$ is velocity $\rm (miles/day)$,  $x$ is distance from point source $\rm (miles)$. There are coefficients for initial concentration $s_0 = 350 \ {\rm mg/L}$ and tide wave dispersion coefficients $E = 5 \ {\rm miles^2/day}$.


## velocity
In a certain estuary the velocity can be formulated as

$$
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
