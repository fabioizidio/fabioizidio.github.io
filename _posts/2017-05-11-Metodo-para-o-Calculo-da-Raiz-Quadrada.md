---
layout: post
title: Metodo para o Cálculo da Raiz Quadrada
description: Uma breve demonstração do método numérico para o cálculo aproximado da raiz quadrada
category: Matemática
headline: Matemática
tags: [Matemática, Análise, Números Irracionais, Raiz Quadrada]
imagefeature: math.jpg
comments: true
mathjax: true 
chart: false
---

A operação de raiz quadrada é uma das mais fundamentais da Matemática e aparece em inúmeras situações, mas infelizmente, ao contrário das operações de adição, subtração, multiplicação, divisão e potenciação, calculá-la às vezes não é óbvia para uma pessoa comum. Apesar de existirem alguns métodos numéricos para fazer tal operação quero trazer uma demonstração que, durante minhas brincadeiras, desenvolvi. Confesso que não sei se alguém já a demonstrou (não lembro de tê-la visto) mas é meu desejo deixar esta contribuição. Então, mãos à obra! 

## O Binômio de Newton e a Desigualdade de Bernoulli

O conhecido Binômio de Newton é definido por: 

$$ (x+y)^n = \sum_{k=0}^n \binom{x}{k}x^{k}y^{n-k} \quad \forall x,\,y \in \mathbb{R}\,\mathrm{e}\,x \in \mathbb{N} $$
