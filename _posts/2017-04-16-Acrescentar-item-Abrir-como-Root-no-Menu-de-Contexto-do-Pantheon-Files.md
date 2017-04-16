---
layout: post
title: Como Acrescentar item "Abrir como Root" no Menu de Contexto do Pantheon-Files
description: "Configurações do Elementary OS"
headline: GNU/Linux
category: GNU/Linux
tags: [Elementary OS, eOS Loki, GNU/Linux, Sistemas Operacionais, Open Source, Personalização, Script]
imagefeature: picture-29.jpg
comments: true
mathjax: false
chart: false
---

Saudações aos linuxusers de plantão!

Nossa dica de hoje é acrescentar alguns comandos ao menu de contexto do pantheon-files. Para deixar claro, esses comandos são aqueles aparecem quando você clica com o botão direito do mouse. Quero deixar aqui dois comandos que julgo importantes: "abrir arquivo como root" e "abrir pasta como root". São importantes porque quando você precisa fazer alguma alteração em um arquivo protegido, não precisa ir ao terminal para lançar algum comando que lhe dê a permissão de administrador. É bem mais prático clicar sobre o arquivo ou pasta e confirmar o comando. Para isso, é preciso criarmos arquivos com a extensão .contract no diretório */usr/share/contractor* em modo administrador. Bem, vamos as dicas!

1 - Abrir Arquivo como Administrador

Vá ao terminal pressionando `< WinKey >+< T >` e digite o comando logo abaixo para abrir o editor de texto scratch em modo administrador:

    $ gksu scratch-text-editor

Em seguida, digite o comando abaixo e depois salve o aquivo no diretório */usr/share/contractor com o nome scratch-openasroot.contract*:

    [Contractor Entry]
    Name=Abrir arquivo como administrador
    Icon=scratch-text-editor
    Description=Abre um arquivo em modo root com o scratch
    MimeType=text
    Exec=gksudo scratch-text-editor %U
    Gettext-Domain=scratch-text-editor

Note que estou usando o *scratch-text-editor* como o aplicativo padrão. Você pode usar outro editor do seu gosto só fazendo as devidas modifcações no arquivo.

2 - Abrir Pasta como Administrador

Este processo é bem semelhante ao anterior. Vá ao terminal e digite o comando logo abaixo para abrir o editor de texto scratch em modo administrador:

    $ gksu scratch-text-editor

Em seguida, digite o comando abaixo e depois salve o aquivo no diretório */usr/share/contractor* com o nome *pantheon-files-openasroot.contract*:

    [Contractor Entry]
    Name=Abrir pasta como administrador
    Icon=pantheon-files
    Description=Abre uma pasta corrente em modo root no pantheon-files
    MimeType=inode
    Exec=gksudo pantheon-files %U
    Gettext-Domain=pantheon-files

Então, galera, esta concluída nossa dica facílima. Testem e aproveitem!

Até a próxima!

Fábio Izidio

