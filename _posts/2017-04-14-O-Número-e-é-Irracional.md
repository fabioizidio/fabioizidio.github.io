---
layout: post
title: O Número e é Irracional
description: Uma breve demonstração da irracionalidade do número neperiano
category: Matemática
headline: Matemática
tags: [Matemática, Análise, Números Irracionais, Número Neperiano, Número e, Cálculo, Exponencial, Logaritmo]
imagefeature: math.jpg
comments: true
mathjax: true 
chart: false
---

# O Número "e" é Irracional

Definamos a função $ \ln:\mathbb{R}^+ \rightarrow \mathbb{R} $
onde, $ \forall x > 0 $ temos \\[ \ln x = \int_1^x \frac{dt}{t}.\\]

A função $ \ln $
subtente a área sob o arco de hipérbole, de modo que $ \ln x $ é a medida da área no intervalo $ [1,x] $ para $ x \geq 1 $ e $ [x,1] $ para $ 0 < x < 1 $. Com isso em mente, podemos definir o número e como sendo o valor assumido por $ x $ quando a área sob o arco da hipérbole é igual a 1.

No Cálculo se demonstra que \\[ e = \sum_{n=0}^{+\infty} \frac{1}{n!}. \qquad \mathrm{(1)} \\]

Para provarmos que $ e $
é irracional, suponhamos por absurdo que $ e $ seja racional, isto é, $ e=\frac{p}{q} $, onde $ p\,q \in \mathbb{N} $ e $ (p,q)=1 $ ($ p $ e $ q $ são primos entre si). Desenvolvendo (1) temos que \\[ \frac{p}{q}−\left (1+\frac{1}{1!}+\frac{1}{2!}+\cdots+\frac{1}{q!} \right )= \sum_{n=q+1}^{+\infty}\frac{1}{n!}. \qquad (2) \\]

Analisando o segundo membro de (2)
temos que \\[ \sum_{n=q+1}^{+\infty} \frac{1}{n!} = \frac{1}{q!}\left ( \frac{1}{(q+1)}+\frac{1}{(q+1)(q+2)}+\cdots \right ) < \frac{1}{q!} \left ( \frac{1}{(q+1)}+\frac{1}{(q+1)^2} + \cdots \right ). \qquad (3) \\]

Agora podemos observar que a expressão entre parêntesis do último membro de (3)
é uma série geométrica de razão pertencente ao intervalo $ (0,1) $. Logo, a série é convergente e converge para $ \frac{1}{q} $. Portanto, \\[ \sum_{n=q+1}^{+\infty} \frac{1}{n!} < \frac{1}{q!} \frac{1}{q}. \qquad (4) \\]

Agora podemos reescrever (2)
como \\[ 0 < \frac{p}{q}− \left (1+\frac{1}{1!}+\frac{1}{2!}+\cdots+\frac{1}{q!} \right ) < \frac{1}{q}\frac{1}{q!} \\] e, consequentemente \\[ 0 < q!\left( \frac{p}{q}−1−\frac{1}{1!}−\frac{1}{2!}−\cdots−\frac{1}{q!} \right ) < \frac{1}{q}. \qquad (5) \\] 

O membro central da desigualdade (5)
é um número inteiro, pois $ q! $ cancela todos os denominadores. Mas como $ q \in \mathbb{N} $, temos que $ \frac{1}{q} < 1 $, chegamos ao absurdo de que existe um número inteiro entre 0 e 1. Tal absurdo provém da afirmação inicial de que o número e é um racional. Portanto, e

é um número irracional.

*Referência:*

- FIGUEREDO, Djairo Guedes de, Números Irracionais e Transcendentes, Sociedade Brasileira de Matemática (SBM), 2002.
- LIMA, Elon Lages, Análise Real, Volume 1, Coleção Matemática Universitária, Instituto Nacional de Matemática Pura e Aplicada (IMPA), 2014.

Tags: Número e, Iracional, Análise, Cálculo, Exponencal, Logarítmo

