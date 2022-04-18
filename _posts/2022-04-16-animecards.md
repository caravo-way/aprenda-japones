---
title: Animecards
date: 2022-04-16 17:23:00 +/-TTTT
categories: [Guia, Teoria]
tags: [guia, teoria, srs, anki]
author: gustavo_maia
comments: false
---

# Introdução

[Animecards](https://animecards.site/) é um modelo de cards para o ANKI criado pela comunidade gringa de aprendizado de japonês.

No geral, existem dois tipos de cards: cards de vocabulário e cards de sentenças. Esse metodo é para quem deseja utilizar **cards de vocabulário.** Recomendo que leia o artigo escrito explicando a diferença entre os dois antes de decidir se quer continuar lendo isso.

Já usei diversos modelos de card e o que uso hoje e recomendo é esse. É um pouquinho chato pra configurar mas no fim, criar cards vai ser bem fácil. Praticamente 1 clique.

> ### Importante!
> 
> Antes que comecem com o cancelamento, entrei em contato com o fundador do site original perguntando o que ele achava de eu passar o conteúdo para português aqui no aprendajp e o que ele disse foi o seguinte:
>
>> Hey,
>>
>> yeah that's no problem. Feel tree to do with the site content whatever you like.
>>
>> Be aware though that some suggestions are not entirely up to date, for example the "Load Balancer" add-on hasn't been updated for the new scheduler and "Straight Rewards" may be redundant with the V3 scheduler. I'll have to look into it and possibly update the guide again.
>>
>> Good luck.
{: .prompt-warning }

Fiquei feliz com a resposta porque ela deixou bem claro que seguimos uma filosofia parecida. Não importa quem entrega o conteúdo, o que veio de forma gratuita deve ser distribuído de forma gratuita.

Com isso esclarecido, vou fazer o possível para deixar esse artigo o mais enxuto possível.

# Configuração do Anki

Configurar o anki é um processo bem chatinho. A parte difícil é entender o que cada uma das opções faz, o que não é muito intuitivo. O programa em sí é bem facil de entender. Como o texto onde explico a configuração ficou muito grande, [escrevi um artigo separado.]({% link _posts/2022-04-16-como-configurar-anki.md %})

# Configurando Yomichan e integração com Anki

Yomichan é uma extensão de browser, com ela, você consegue ter um "on-hover pop-up dictionary". Isso é, passar o mouse por cima de uma palavra em japonês e ver um mini dicionário ao lado dela.

![image](https://user-images.githubusercontent.com/19489884/163693592-9769cd17-49b7-4bd2-9a14-e6642a1065b6.png)

O maior problema é justamente o que você está vendo na imagem. Todos os dicionários que eu conheço e gosto são em inglês e é humanamente impossível traduzir isso sem ser de forma automática. Tem jeito, tocarei nesse assunto mais a frente.

## Instalando Yomichan

Extensão: [Chrome](https://chrome.google.com/webstore/detail/yomichan/ogmnaimimemjmbakcfefmnahgdfhfami) [Firefox](https://addons.mozilla.org/en-US/firefox/addon/yomichan/)

Instale o [AnkiConnect](https://ankiweb.net/shared/info/2055492159)

O AnkiConnect é um adicional pro anki que permite com que ele se comunique com o Yomichan.

Ferramentas → Extensões → Obter Extensões → Código: 2055492159 → OK → Reinicie o Anki após a instalação.

## Instalando dicionários no Yomichan

Se você falar inglês, pegue seus dicionários [aqui.](https://foosoft.net/projects/yomichan/index.html#dictionaries)

Instale os seguintes dicionários:

* jmdict_english
* kanjidic_english
* kanjium_pitch_accents (só confia)

Agora vem a parte complicada. Se você só fala português, nos resta apenas a gambiarra. [Uma pessoa bem intencionada](https://github.com/eyeS-Code/jmdict_portuguese) traduziu o JMDict para português utilizando o Deepl, que é um bom tradutor.

Ativei o dicionário em português para escrever esse artigo e esqueci ligado, comecei a fazer cards usando ele sem querer, ou seja, a tradução esta tão boa que eu nem percebi! As instruções de instalação desse dicionário estão na descrição do projeto dele.

Instale tambem o kanjium_pitch_accents citado acima.

## Conectando com o Anki

Abra o Yomichan e habilite a opção "Enable Anki Integration"

Clique em "Configure Anki card format..."

Selecione o seu deck e model. Se ainda não tiver nenhum, baixe [esse deck](https://ankiweb.net/shared/info/151553357) de template.

## Handlebars

Apenas saiba que pulando essa etapa, seus cards ficarão uma bagunça.

* Ative as opções avançadas do yomichan.

![image](https://user-images.githubusercontent.com/19489884/163694078-f714a03e-c2f9-4118-b4d2-24ad333566ce.png)

* Vá em ```Configure Anki card format``` e substitua {glossary} ou {glossary-brief} por {test}

* Vá em ```configure Anki card Templates``` e substitua o texto lá por esse [aqui](https://pastebin.com/TeSJc6ij)

## Configurações do Card

Adicione os seguintes campos no seu ```Configure Anki card format```

front: {expression} - Palavra alvo

Reading: {reading} - Leitura da palavra

Glossary: {pitch-accent-positions} {test} - Indicação numérica e visual de ```pitch accent```.

Audio: {audio} - Pronúncia da palavra

Graph: {pitch-accent-graphs} - Gráfico do ```pitch accent```

> Não esquenta com o que é ```pitch accent``` agora, sério. O seu Eu do futuro irá me agradecer, mas o de agora não precisa entender nada!
{: .prompt-info }

![image](https://user-images.githubusercontent.com/19489884/163694315-118a1937-9c56-48bc-abed-14bb04bee155.png)

Se estiver tudo certo, o seu resultado será esse:

![image](https://user-images.githubusercontent.com/19489884/163694533-1d40abf7-c1f4-4551-bf3a-18e72735a6ac.png)

Ao clicar no botão de +, um card é criado no anki automaticamente. Exemplo:

![image](https://user-images.githubusercontent.com/19489884/163694557-ea100180-a1dc-48b8-8c94-01240701b601.png)

Agora você já consegue criar cards bem simples com 1 clique. Em um próximo artigo, vou ensinar a fazer isso com qualquer conteúdo que esteja assistindo, com imagem, vídeo e áudio, dessa forma:

![image](https://user-images.githubusercontent.com/19489884/163694637-7a2b0d63-59a3-48b8-9fd0-05ff72b0d443.png)

> Thanks again to the guys at [animecards](http://animecards.site) <3.
{: .prompt-info }