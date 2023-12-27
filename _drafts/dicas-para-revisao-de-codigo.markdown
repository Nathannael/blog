---
layout: single
title:  "Dicas para revisão de código"
excerpt: "Dicas e crenças que uso no meu dia-a-dia revisando código e podem ajudar outras pessoas."
date: 2023-06-04 20:17:21 -0300
categories: desenvolvimento
header:
  overlay_image: assets/images/spotify/sgcdesignco-NIo8Fd-RngE-unsplash.jpg
  overlay_filter: 0.6
  caption: "Photo by [**sgcdesignco**](https://unsplash.com/@sgcreative) on [**Unsplash**](https://unsplash.com/photos/NIo8Fd-RngE)"

---

Por todas as empresas que passei, e acredito que em grande parte das equipes de desenvolvimento atualmente, a revisão de código sempre foi uma parte importante do processo de trabalho. A efetividade e investimento da prática variam muito. Alguns times, principalmente se influenciados por desenvolvedores de senhoridade alta e líderes técnicos, tratam a presença dessa prática como essencial para que o trabalho seja tratado como completo. Para outros times, especialmente os com menos expertise em metodologias ágeis ou lideranças menos técnicas, tratam como uma forma de "cumprir tabela", mas sem dar muito julgamento quanto à sua importância. Na comunidade em geral, a revisão de código nem sempre é tratada com unanimidade. Existem vários posts defendendo que eles machucam a produtividade do time e que deveríamos confiar mais no trabalho de nossos colegas.

Eu não sou um dos que condenam a revisão de código. Para mim, é uma ferramenta indispensável que um time tem de disseminar conhecimento entre seus colaboradores. Os benefícios são claros: nem sempre temos tempo de ficar a par de tudo o que acontece num time, mas ao revisar o trabalho de outro desenvolvedor, você fica ciente do que ele fez e porque ele o fez. Esse momento também favorece várias possibilidades de crescimento e interação no time:

- É uma oportunidade de aprendizado: Você pode entender mais sobre uma nova funcionalidade do projeto, ou sobre a linguagem utilizada no dia-a-dia. Todos escrevem código de forma diferente e observar como um colega de trabalho resolveu um problema pode te fazer pensar de novas formas;
- É uma oportunidade de mentoria: Da mesma forma que você tem muito a aprender algo novo com o código dos seus colegas de time, eles também tem muito a aprender com os seus. Sessões de revisão de código podem ser ótimas formas de apresentar conceitos, mostrar funcionalidades importantes de uma linguagem ou framework, ou oferecer novas formas de pensar o problema. Todo mundo ganha!
- É uma chance de corrigir problemas antes que eles aconteçam: mesmo os melhores desenvolvedores cometem erros. Uma consulta mal otimizada, um debugger esquecido, uma lógica que vai contra a forma como o sistema funciona. Ter ajuda de outras pessoas do time com um olhar externo ajuda a identificar problemas que talvez você deixou passar por estar muito focado no que tem que entregar.

Eu credito uma grande parte da evolução da minha carreira a revisões de código, tanto as que eu realizei quanto as que eu recebi. Ao longo do tempo, solidifiquei algumas ideias e vi muitos padrões que ajudaram a ser mais efetivo nesse exercício. A seguir, falarei sobre alguns tópicos que acho importante ter em mente quando revisando, e darei algumas dicas que me ajudam diariamente a entrar numa mentalidade de ser construtivo e ajudar meu time. Mas antes, algumas clarificações:

-  Vou tratar aqui principalmente da revisão de código que acontece em _Pull Requests_ (PRs). Revisão de código pode ser feita de várias formas, inclusive em sessões de **programação em par** que tendem a ser muito benéficas, mas a revisão de PR como etapa no fluxo de desenvolvimento é bem comum no meu dia-a-dia e acredito que no dia-a-dia de muitos outros desenvolvedores.
- Grande parte dos tópicos a seguir foram inspiradas num episódio do podcast [Developer Tea](https://pod.link/955596067), que já indiquei na minha lista de Podcasts preferidos [(link)](https://www.nathann.dev/blog/indica%C3%A7%C3%B5es/podcasts/#developer-tea). Recomendo bastante a escuta desse episódio e do podcast em geral.

- Be curious, not judgemental