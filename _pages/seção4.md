---
title: "Tutorial para o uso do software Insight Maker"
excerpt: "Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit"
permalink: /secao4/
layout: single
author_profile: false
mathjax: true
header:
  overlay_color: "#98d6ea"
sidebar:
  title: " "
  nav: insightmaker
---
# Instruções para construir o seu modelo no Insight Maker

Para construir um modelo no _Insight Maker_, o primeiro passo é criar uma conta livre na página
inicial do programa <a href="https://insightmaker.com">https://insightmaker.com</a> (Veja a Figura 1.4). Basta entrar na opção
_Create a free account_, no canto superior direito da página, e preencher algumas informações no
formulário que se abrirá. Uma dessas informações é sua conta de _email_ e uma senha de sua escolha.
Então, acesse o _log in_, no canto superior direito da página, para entrar na área de criação de modelos,
e prossiga com as orientações abaixo.
{: .text-justify}

![Figura 1.4: Página inicial do Insight Maker.]({{ site.url }}{{ site.baseurl
}}/assets/images/ACCOUNT.png){: .align-center}   

{: .image-caption}
*Figura 1.4: Página inicial do Insight Maker.*
 {: .text-center} 

Ao fazer login no _Insight Maker_ pela primeira vez, clique em _Create New Insight_ (no canto
superior direito). Aparecerá a imagem que você vê na Figura 1.5. Clique, então, em _Click me to
clear this Demo Model_ (no canto superior direito). Agora você tem à sua disposição a área para
criação de modelos.
{: .text-justify}

![Figura 1.5: Botão para gerar uma área para criação de modelos]({{ site.url }}{{ site.baseurl
}}/assets/images/CLICK.png){: .align-center}   

{: .image-caption}
*Figura 1.5: Botão para gerar uma área para criação de modelos.*
 {: .text-center}

Para implementar o modelo mostrado na Figura 1.3, adicione os estoques do modelo usando
o comando _Add primitive_ (topo esquerdo da tela do computador), e opte por _Add Stock_. Crie um
estoque para os <span style="font-family: Comic Sans MS">Livros na biblioteca</span> e outro para os <span style="font-family: Comic Sans MS">Livros emprestados</span>. Mova os retângulos que
representam os estoques para a região da tela que julgar mais conveniente. Note que com o cursor
em cima do retângulo, você vê uma setinha azul no meio do retângulo, e um sinal de igual no centro
de uma bolinha cinza do lado esquerdo. Esses sinais lhes serão muito úteis.
{: .text-justify}

Para conectar os estoques formados, precisamos criar um fluxo. Na Figura 1.6 está explicado
como criar um fluxo e avaliar se ele está devidamente conectando um estoque ao outro.
{: .text-justify}

![Figura 1.6: Passos para a criação de fluxos.]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOW1.png){: .align-center}   

{: .image-caption}
*Figura 1.6: Passos para a criação de fluxos.*
 {: .text-center}
 
Já na Figura 1.7 está indicado como modificar o formato do fluxo para que ele seja igual ao da
Figura 1.3.

![Figura 1.7: Modificação do formato do fluxo]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOWCHANGE.png){: .align-center}   

{: .image-caption}
*Figura 1.7: Modificação do formato do fluxo*
 {: .text-center}

Clicando duas vezes sobre o retângulo, elipse e seta você pode atribuir os nomes dos estoques,
variáveis e fluxos: por ex., <span style="font-family: Comic Sans MS">Livros na biblioteca</span>. Com o cursor em cima do estoque de <span style="font-family: Comic Sans MS">Livros na biblioteca</span>, estenda a setinha azul para criar o fluxo que representa os empréstimos diários, ou seja,
que vai do estoque de <span style="font-family: Comic Sans MS">Livros na biblioteca</span> para o estoque <span style="font-family: Comic Sans MS">Livros emprestados</span>. Faça o mesmo para
criar o outro fluxo, que é das <span style="font-family: Comic Sans MS">Devoluções</span> e que tem o sentido inverso do fluxo de <span style="font-family: Comic Sans MS">Empréstimos</span>.
{: .text-justify}

Novamente em _Add primitive_, opte por _Add variables_ para criar as variáveis <span style="font-family: Comic Sans MS">Prazo para devolução</span> e <span style="font-family: Comic Sans MS">Porcentagem de empréstimos</span>.
{: .text-justify}

Observe também que no topo da área de trabalho do _software_ vê-se a Figura 1.8. A cor cinza
escuro indica que é o comando _Flows_ que está ativo. Clicando em _Links_, ficará cinza escuro, e será
possível criar um _link_. Clicando nas setinhas à direita se pode inverter o sentido de fluxos.
{: .text-justify}

![Figura 1.8: Comandos para a criação de fluxos e links.]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOW-LINKS.png){: .align-center}   

{: .image-caption}
*Figura 1.8: Comandos para a criação de fluxos e links.*
 {: .text-center}

Finalmente, clique em _Links_ e siga os passos da Figura 1.9 para criar o _link_ entre cada variável
e o fluxo que ela influenciará.
{: .text-justify}

![Figura 1.9: Comandos para criação de links.]({{ site.url }}{{ site.baseurl
}}/assets/images/LINK.png){: .align-center}   

{: .image-caption}
*Figura 1.9: Comandos para criação de links.*
 {: .text-center}

Você deve ter conseguido reproduzir a Figura 1.3. Resta agora introduzir as equações que
relacionam essas grandezas, assim como os valores iniciais.
{: .text-justify}

Já vimos que o fluxo de <span style="font-family: Comic Sans MS">Devoluções</span> é igual à <span style="font-family: Comic Sans MS">Livros emprestados</span> dividido pelo valor da variável
<span style="font-family: Comic Sans MS">Prazo para devolução</span>, que tomaremos igual a 7.
{: .text-justify}

Para introduzir essas informações no modelo, basta proceder como mostrado na Figura 1.10.
{: .text-justify}

![Figura 1.10: Visualização da criação de fluxos.]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOW.png){: .align-center}   

{: .image-caption}
*Figura 1.10: Visualização da criação de fluxos.*
 {: .text-center}
 
Já o fluxo de livros que sai da biblioteca (<span style="font-family: Comic Sans MS">Empréstimos</span>) será igual ao valor do estoque de
<span style="font-family: Comic Sans MS">Livros na biblioteca</span> vezes o valor da variável <span style="font-family: Comic Sans MS">Porcentagem de empréstimos</span>. Para introduzir essas
informações no modelo, basta proceder como mostrado na Figura 1.11.
{: .text-justify}

![Figura 1.11: Visualização da criação de fluxos.]({{ site.url }}{{ site.baseurl
}}/assets/images/FLOW2.png){: .align-center}   

{: .image-caption}
*Figura 1.11: Visualização da criação de fluxos.*
 {: .text-center}
 
Vamos agora inserir o valor 0.03 para a variável <span style="font-family: Comic Sans MS">Porcentagem de empréstimos</span>. Para isso, clique
em cima na elipse que representa essa variável. Ao fazer isso abre-se uma barra lateral à direita da
área de trabalho do _software_ onde você preencherá ao lado de _Value/Equation_ o valor 0.03. Note
que no _Insight Maker_ é usado ponto para separar as casas decimais, não vírgula. Cuidado para não
utilizar vírgula!
{: .text-justify}

Falta inserir o valor da outra variável. O processo é semelhante ao recém executado. Clique
em cima da elipse que representa a variável <span style="font-family: Comic Sans MS">Prazo para devolução</span> e coloque o valor 7 no campo
Value/Equation.
{: .text-justify}

Resta colocar o valor inicial nos estoques. Clique em cima do retângulo que representa cada
estoque e coloque o número inicial de <span style="font-family: Comic Sans MS">Livros na biblioteca</span> igual à 1100 e valor inicial de <span style="font-family: Comic Sans MS">Livros emprestados</span> igual à 350.
{: .text-justify}
 

[<i class="fas fa-arrow-alt-circle-left"></i> Seção 3 ](https://milenalauschner.github.io/TutorialIM/secao3/){:
.btn .btn--warning} [ Seção 5 <i class="fas fa-arrow-alt-circle-right"></i>](https://milenalauschner.github.io/TutorialIM/secao5/){:
.btn .btn--info}
 {: .text-right}
________________________________________________________________________________________________________________________________________________________________________________________________ 
 
