---
title: "Como usar e configurar o anki: Limites, falhas e configurações avançadas!"
date: 2022-04-16 19:22:00 +/-TTTT
categories: [Guia, Teoria]
tags: [guia, teoria, srs, anki]
author: gustavo_maia
comments: false
---

# Entendendo as configurações do Anki.

Anki é uma das melhores ferramentas para o aprendizado de qualquer língua, não só o japonês. O algoritmo funciona muito bem e, se bem configurado e se seguir a metodologia correta, você poderá aproveitar mais e se frustrar menos.

> Se quiser entender melhor como e porque o algoritmo do Anki funciona, recomendo que leia o artigo: [O papel do SRS]({% link _posts/2022-01-22-O papel do SRS.md %})
{: .prompt-info}


Essas são as minhas configurações, especialmente pensadas para utilizar o modelo de cards [desse artigo.]({% link _posts/2022-04-16-animecards.md %}) Se não estiver afim de ler o artigo inteiro, no final dele vou deixar um print das minhas configurações.

## Limites Diários

### Novos cartões/dia

Isso depende de quanto tempo você quer dedicar ao anki por dia. Usando esse método que estamos ensinando, 20 cards novos por dia é um número ótimo, o ritmo de aprendizado é bem rápido e não toma muito tempo por dia. 10 cards por dia é um número bom, bem mais casual e sustentável. No longo prazo também te trará bons resultados.

Tome cuidado para não fazer muitos cards novos por dia. O volume de revisões real só chega no pico depois de aproximadamente uma semana e meia, é muito fácil começar fazendo 50 cards por dia para depois descobrir que você não dá conta das revisões. Um dia pulado acumula para o próximo e sair disso é **bem difícil.**

Recomendo que comece fazendo 10 cards por dia por duas semanas. Se estiver conseguindo fazer suas reviews e cards novos tranquilamente ou pensar que está difícil demais, mude o número de acordo.

Mais do que 20 cards por dia ja seria demais para mim, por exemplo. Me tomaria muito tempo diariamente (mais de uma hora) e me deixaria bem cansado, tome cuidado para não entrar no *anki hell.*

> **Minha recomendação:** Comece com 10 e após duas semanas aumente ou diminua conforme a sua preferência.
{: .prompt-tip }

### Revisões máximas/dia 

Como estamos regulando isso conforme o número de novos cartões por dia, pode colocar 9999!

## Cartões novos

### Learning steps 

Esse valor define quantas etapas serão necessárias para um cartão novo ser graduado e remarcado para a próxima data.

Eu utilizo 3 etapas, então minha configuração é: 1m 5m 1h

Isso significa que se você marcar o card como correto, ele será mostrado novamente após 5 minutos. Se você marcar ele como correto novamente, ele será mostrado novamente depois de uma hora e no fim da sessão você aprova ele uma ultima vez. Se você falhar o card, ele é mostrado novamente após um minuto.

Tenha em mente que você não precisará esperar uma hora até o card ser mostrado novamente caso sua sessão não dure tudo isso, eles serão simplesmente mostrados por último na sua sessão.

> Minha recomendação: 1m 5m 1h
{: .prompt-tip }

## Falhas

### Relearning steps 

O mesmo de learning steps, mas para os cards que você falhou. Como é apenas algo que já sabe e apenas errou, deixo menos etapas: 2m e 60m. Assim, Reviso uma vez no começo e no final da sessão.

> **Minha recomendação:** 2m 1h 
{: .prompt-tip }

### Ação sanguessuga  

Só para que não fique dúvida, uma sanguessuga ou _leech_ como vou chamar daqui para frente é um card que por algum motivo você tem dificuldades para lembrar. É um card que você ja aprendeu e esqueceu diversas vezes, ele apenas suga a sua energia tentando aprende-lo. Cards assim eu prefiro apenas suspender. Então, coloco suspender cartão. Assim, se um card se torna um _leech_ ele é simplesmente retirado do meu deck.


## Avançado

### Intervalo máximo 

Isso não nos interessa, o que o algoritmo definir está bom. Deixo o meu 36500.

### Facilidade Inicial

É o multiplicador que define o intervalo dos cards que você acertou. Um valor maior significa que o intervalo entre as revisões é maior. Mais para frente pretendo escrever um artigo só sobre _ease_, por enquanto, apenas saiba que isso define o valor inicial do multiplicador, deixe o padrão de 2.5

### Modificador de intervalo

Esse é o multiplicador constante que define o intervalo dos cards (A opção acima é apenas o valor inicial)

O valor padrão é ok. Eu pessoalmente tenho uma memória horrível, então deixo o meu em 0.8, o que significa que meus intervalos são menores e, portanto, mais reviews por dia.

Aumentar esse valor deixa suas reviews mais tranquilas no curto prazo, mas recomendo que comece no valor padrão: 1

### Novo intervalo

Esse valor define o intervalo de cards que você já sabia, mas falhou. Deixar em 20% significa que falhar um card que estava com intervalo de 100 dias reverte o intervalo dele para 20 dias. Eu uso 20%

## Minhas configurações

![config 1](https://user-images.githubusercontent.com/19489884/163694667-ffded9c0-ef88-4c8f-a767-b8a26f8155aa.png)

![config 2](https://user-images.githubusercontent.com/19489884/163694668-0e05f0c4-d8f0-46e4-a69e-60f49ff46634.png)
