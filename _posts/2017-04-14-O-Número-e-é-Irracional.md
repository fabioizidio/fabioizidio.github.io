---
layout: post
title: O Número e é Irracional
description: Uma breve demonstração do número neperiano
category: Matemática
headline: Matemática
tags: [Matemática, Análise, Números Irracionais, Número Neperiano, Número e]
imagefeature: math.jpg
comments: true
mathjax: true 
chart: false
---

# O Número "e" é Irracional

Definamos a função $ \ln:\mathrm{R}^+ \rightarrow \mathrm{R} $
onde, $ \forall x > 0 $ temos $$ \ln x = \int_1^x \frac{dt}{t}.$$

A função ln
subtente a área sob o arco de hipérbole, de modo que lnx é a medida da área no intervalo [1,x] para x≥1 e [x,1] para 0<x<1. Com isso em mente, podemos definir o número e como sendo o valor assumido por x

quando a área sob o arco da hipérbole é igual a 1.

No Cálculo se demonstra que e=+∞∑n=01n!(1).

Para provarmos que e
é irracional, suponhamos por absurdo que e seja racional, isto é, e=pq, onde p,q∈N e (p,q)=1 (p e q são primos entre si). Desenvolvendo (1) temos que pq−(1+11!+12!+⋯+1q!)=+∞∑n=q+11n!(2).

Analisando o segundo membro de (2)
temos que +∞∑n=q+11n!=1q!(1(q+1)+1(q+1)(q+2)+⋯)<1q!(1(q+1)+1(q+1)2+⋯)(3).

Agora podemos observar que a expressão entre parêntesis do último membro de (3)
é uma série geométrica de razão pertencente ao intervalo (0,1). Logo, a série é convergente e converge para 1q. Portanto, +∞∑n=q+11n!<1q!1q(4).

Agora podemos reescrever (2)
como 0<pq−(1+11!+12!+⋯+1q!)<1q1q! e, consequentemente 0<q!(pq−1−11!−12!−⋯−1q!)<1q(5).

O membro central da desigualdade (5)
é um número inteiro, pois q! cancela todos os denominadores. Mas como q∈N, temos que 1q<1, chegamos ao absurdo de que existe um número inteiro entre 0 e 1. Tal absurdo provém da afirmação inicial de que o número e é um racional. Portanto, e

é um número irracional.

*Referência:*

- FIGUEREDO, Djairo Guedes de, Números Irracionais e Transcendentes, Sociedade Brasileira de Matemática (SBM), 2002.
- LIMA, Elon Lages, Análise Real, Volume 1, Coleção Matemática Universitária, Instituto Nacional de Matemática Pura e Aplicada (IMPA), 2014.

Tags: Número e, Iracional, Análise, Cálculo, Exponencal, Logarítmo

