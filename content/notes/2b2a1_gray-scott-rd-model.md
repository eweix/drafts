---
title: gray-scott model
aliases:
  - gray-scott model
tags: null
date: 2023-08-15
---

## Equations[^1]
The Gray Scott Model describes [[notes/2b2a_reaction-diffusion-systems-self-organize|reaction-diffusion systems]] using the following equations:
$$\frac{\partial u}{\partial t} = F(1-u) - uv^{2}+ D_{u}\Delta^{2}u$$
$$\frac{\partial v}{\partial t} = -(F+k)v + uv^{2}+ D_{u}\Delta^{2}v$$

This model assumes the following autocatalytic reaction:
$$\ce{ u + 2v -> 3v }$$
The reaction takes a single unit of $u$ and converts it into one unit of $v$. The reaction is autocatalyic because it requires two units of $v$ to take place. Some external source replenishes $u$ up to 1 at feed rate $F$, and $v$ is continuously removed from the system slightly faster than $u$ is replenished ($F+k$). 

## Implications

[^1]: Equations taken directly from [libretexts](https://math.libretexts.org/Bookshelves/Scientific_Computing_Simulations_and_Modeling/Book%3A_Introduction_to_the_Modeling_and_Analysis_of_Complex_Systems_(Sayama)/13%3A_Continuous_Field_Models_I__Modeling/13.06%3A_Reaction-Diffusion_Systems)