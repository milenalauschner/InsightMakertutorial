---
title: "Tutorial para o uso do software Insight Maker"
excerpt: "Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit"
layout: single
permalink: /secao2/
layout: single
author_profile: false
mathjax: true
header:
  overlay_color: "#ddf3f5"
sidebar:
  title: " "
  nav: insightmaker
---

# Introdução ao uso do Insight Maker

Para facilitar a compreensão do funcionamento do _Insight Maker_, vamos descrever a lógica de construção de modelos neste _software_, e as suas principais características, nos valendo de um exemplo comum na vida de um estudante: uma biblioteca com uma coleção de livros que são cedidos por empréstimo aos estudantes da escola.
{: .text-justify}

Vamos querer responder questões do tipo: 

  * Quantos livros permanecem na biblioteca depois de certo tempo? 
  * Qual é o percentual de livros emprestados em determinado dia? 

Para isso vamos construir um modelo sobre o estoque de livros na biblioteca levando em conta que há empréstimos e devoluções. Como todo modelo, ele não representa exatamente o sistema em estudo. Trata-se de uma representação simplificada do sistema real, que poderá ser aprimorada na medida dos nossos interesses e conhecimentos sobre o sistema em estudo. 
{: .text-justify}

Considere que há certa quantidade de livros disponíveis em uma biblioteca, ou seja, tem um estoque de livros. Digamos que em certo momento haja $$n$$ livros na biblioteca. Essa quantidade de livros pode diminuir porque alguns livros são emprestados aos alunos, assim como pode aumentar porque alguns livros que estavam emprestados são devolvidos. Um diagrama que representa o número de livros na biblioteca é visto na Figura 1.1, onde o retângulo representa o estoque de livros. As setas representam livros que entram ou saem da biblioteca. A seta da esquerda, apontando para dentro do retângulo, indica que há um fluxo de livros entrando no estoque da biblioteca (devoluções de livros pelos alunos). A da direita, apontando para fora do retângulo, indica que há um fluxo de livros saindo do estoque da biblioteca (empréstimos de livros para alunos).
{: .text-justify}

![Figura 1.1: Diagrama stock-flow da biblioteca.]({{ site.url }}{{ site.baseurl
}}/assets/images/BIBLIOTECA1.png){: .align-center}   

{: .image-caption}
*Figura 1.1: Diagrama stock-flow da biblioteca.*
 {: .text-center} 

[<i class="fas fa-arrow-alt-circle-left"></i> Seção 1](https://milenalauschner.github.io/TutorialIM/){:
.btn .btn--primary}[ Seção 3 <i class="fas fa-arrow-alt-circle-right"></i>](https://milenalauschner.github.io/TutorialIM/secao3/){:
.btn .btn--warning}
{: .text-right} 
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

