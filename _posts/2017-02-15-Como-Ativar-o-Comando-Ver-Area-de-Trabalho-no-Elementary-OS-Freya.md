---
layout: post
title: "Como Ativar o Comando \"Ver Área de Trabalho\" no Elementary OS Freya"
description: "MathJax Test article"
headline: Elementary OS
category: GNU/Linux
tags: [Elementary OS, GNU/Linux, Personalização, Script]
imagefeature: picture-26.jpg
comments: 
mathjax: 
chart: 
---

Saudações, linuxusers! Nossa dica de hoje será como ativar o comando "mostrar área de trabalho" no Elementary OS Freya, isto é, como minimizar todas as janelas ativas com um único comando no teclado. Confesso que a falta desse comando no eOS foi terrível para mim que estava migrando recentemente do Windows. Pressionar `< WinKey > + < D >` sempre tornou meu trabalho produtivo (`< WinKey >` é a famosa "tecla do Windows"). Espero ajudá-los nas próximas linhas.

Antes de tudo, é preciso que o sistema esteja atualizado. Para isso, pressione `< WinKey > + < T >` para acessar o terminal e em seguida digite os seguintes comandos:

{% raw %}
    $ sudo apt-get update
    $ sudo apt-get dist-upgrade
{% endraw %}

Após encerrar o processo de atualização do sistema, vamos instalar o comando **wmctrl**. Ele serve para fazer o controle de janelas. É nele que reside a mágica para mostrar a área de trabalho de nosso sistema. Para instalá-lo, digite o comando abaixo:

{% raw %}
    $ sudo apt-get install wmctrl
{% endraw %}

Pronto! Temos tudo o que precisamos para que o nosso comando funcione. A próxima etapa é criar um script que encapsule nosso comando. Abra o gerenciador de arquivos do Elementary OS em modo root (administrador) no diretório */usr/local/bin*:

{% raw %}
    $ sudo su
    # pantheon-files /usr/local/bin
{% endraw %}

Agora crie um arquivo chamado **show-desktop** e edite-o usando um editor de texto do seu gosto (o *scratch* por exemplo) inserindo o seguinte código de script:

{% raw %}
    #!/bin/sh
    if wmctrl -m | grep 'mode: ON'; then
        exec wmctrl -k off
    else
        exec wmctrl -k on
    fi
{% endraw %}

Salve o arquivo. Em seguida, no terminal, insira o comando à seguir para tornar o script **show-desktop** executável:

{% raw %}
    $ sudo chmod +x /usr/local/bin/show-desktop
{% endraw %}

Feito tudo isso, vá para **Configurações do Sistema --> Teclado --> Atalhos --> Custom** e adicione o script **show-desktop** e como tecla aceleradora pressione `< WinKey > + < D >`. Pronto! Agora é só encerrar a sessão e efetuar novamente login para usufruir do comando `< WinKey > + < D >` para visualizar a sua área de trabalho.

Até a próxima dica!!!

