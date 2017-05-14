---
layout: post
title: Método para o Cálculo da Raiz Quadrada
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

Expandindo o binômio temos que:

$$ (x+y)^n = \binom{n}{0}x^{0}y^{n} + \binom{n}{1}x^{1}y^{n-1} + \binom{n}{2}x^{2}y^{n-2} + \cdots + \binom{n}{n}x^{n}y^{0} $$

Se eliminarmos do 2o membro todos os termos à partir do 3o termo construímos a seguinte desigualdade: 

$$ (x+y)^n \geq y^n + nxy^{n-1} $$

Fazendo $ y = 1 $ e $ x = h $ construímos a chamada Desigualdade de Bernoulli:

$$ (1+h)^n \geq 1 + nh $$

## A raiz quadrada aproximada

Para o caso de $ n = 2 $ a desigualdade acima fica $ (1+h)^2 \geq 1+2h $. À partir desta última equação, façamos a substituição $ r = 2h $ e teremos $ (1+r/2)^2 \geq 1+r $. Por fim, obteremos:

$$ \sqrt{1+r} \leq 1+r/2. $$

Sejam $$ x \in \mathbb{R} $$ e $$ a,\, b \in \mathbb{N} $$ consecutivos de modo que $$ a^2 \leq x \leq b^2 $$ e $$ x = a^2 + r $$, com $$ |r| < 1 $$. Assim temos que:

$$ \sqrt{x} = \sqrt{a^2+r} = \sqrt{a^2\left (1 + \frac{r}{a^2}\right )} = a\sqrt{1 + \frac{r}{a^2}}. $$

Assim, temos que:

$$ \sqrt{x} = a\sqrt{1 + \frac{r}{a^2}} \leq a\left ( 1 + \frac{r}{2a^2} \right) = a\left ( \frac{2a^2+r}{2a^2} \right). $$

Sabendo que $$ r = x - a^2 $$ notamos que:

$$ a\frac{2a^2-r}{2a^2} = a\frac{2a^2+(x-a^2)}{2a^2} = \frac{x+a^2}{2a}. $$

Portanto, concluímos que 

$$ \sqrt{x} \approx \frac{x+a^2}{2a}. $$

Como queríamos demonstrar. 

## Aplicação

Vejamos agora o uso da nossa fórmula, que torna o cálculo aproximado da raiz quadrada acessível quando não dispomos de calculadoras. 

*Exemplos:*
1. $$ \sqrt{7} $$
Temos que $$ x = 7 $$ e $$ a^2 = 4 \rightarrow a = 2 $$. Logo, 
$$ \sqrt{7} \approx \frac{7+4}{2\cdot2} = \frac{11}{4} = 2,75 $$

Na calculadora $$ \sqrt{7} \approx 2,64575 $$.

2. $$ \sqrt{23} $$
Temos que $$ x = 23 $$ e $$ a^2 = 16 \rightarrow a = 4 $$. Logo, 
$$ \sqrt{23} \approx \frac{23+16}{2\cdot4} = \frac{39}{8} = 4,875 $$

Na calculadora $$ \sqrt{23} \approx 4,79583 $$.

3. $$ \sqrt{123} $$
Temos que $$ x = 123 $$ e $$ a^2 = 121 \rightarrow a = 11 $$. Logo, 
$$ \sqrt{123} \approx \frac{123+121}{2\cdot11} = \frac{244}{22} = 11,091 $$

Na calculadora $$ \sqrt{123} \approx 11,09053 $$.

Observa-se que os resultados são mais próximos do valor real quando a distância entre $$ x $$ e $$ a^2 $$ é a menor possível. 

Encerramos por hoje e até a próxima dica. 

