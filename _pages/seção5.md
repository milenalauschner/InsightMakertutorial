---
title: "Tutorial para o uso do software Insight Maker"
excerpt: "Milena Lauschner Lopes, Leonardo Albuquerque Heidemann e Eliane Angela Veit"
permalink: /secao5/
layout: single
author_profile: false
mathjax: true
header:
    overlay_color: "#86c1d4"
sidebar:
  title: " "
  nav: insightmaker
---
# Algoritmo de análise

Uma vez que o modelo  já está implementado no _Insight Maker_ e já se atribuiu valores iniciais aos estoques, fluxos e variáveis, podemos observar como o sistema dinâmico evolui com o tempo. 
{: .text-justify}

  Para isso é necessário clicar em _Settings_ e aparecerá uma janela como mostrado na Figura 1.12.
É necessário definir o tempo inicial e final da simulação em _Simulation Start/ Simulation Length_
e a unidade do tempo (_Time Units_). No presente caso usaremos dias (_days_) como a unidade de tempo.
{: .text-justify}

![Figura 1.12: Visualização da configuração da simulação.]({{ site.url }}{{ site.baseurl
}}/assets/images/SIMULAR.png){: .align-center}   

{: .image-caption}
*Figura 1.12: Visualização da configuração da simulação.*
 {: .text-center}
 
O método de integração pode ficar no valor de _default_: Método de Euler. Esse é o método
que o bibliotecário utilizou para construir a Tabela 1.2, mesmo sem ter noção sobre métodos de integração. O Método de Euler é o método de integração mais simples que existe, bastante intuitivo, e que serve para muitos propósitos (Asano, 2009).
{: .text-justify}

 Clica-se em _Apply_ e a simulação está pronta para ser rodada clicanco em _Simulate_. 
{: .text-justify}
 
 Para ver os resultados da simulação, depois de clicar em _Simulate_, é preciso entrar em _Add
Display_. Surge uma janela como a mostrada na Figura 1.13. Aí você definirá se quer mostrar uma
Série Temporal (_Time Series_), um gráfico de dispersão (_Scatter Plot_), tabela (_Table_) ou um _Agent
Map_.
{: .text-justify}

![Figura 1.13: Configurações possíveis para representar os resultados do modelo.]({{ site.url }}{{ site.baseurl
}}/assets/images/DISPLAY.png){: .align-center}   

{: .image-caption}
*Figura 1.13: Configurações possíveis para representar os resultados do modelo.*
 {: .text-center}
 
 Queremos organizar os resultados na forma de gráficos ou tabelas. Para fazer uma tabela,
precisamos clicar em _Table_, digitar um título no campo de escrita _Title_ e escolher as componentes
que aparecerão na tabela, chamado pelo _software_ de _Data_ - em português, dado. Após isso, é só confirmar o nova criação no botão _Apply_ (Aplicar).
{: .text-justify} 
 
Os passos descritos para criação de uma tabela estão indicados na Figura 1.14. A tabela para
o modelo da biblioteca é a Figura 1.15. Nela são mostrados os valores obtidos para o número
de <span style="font-family: Comic Sans MS">Livros na biblioteca</span> e de <span style="font-family: Comic Sans MS">Livros emprestados</span> nos <span style="font-family: Comic Sans MS">dias</span> 0,1,2,3..., além dos <span style="font-family: Comic Sans MS">Empréstimos</span> e das
<span style="font-family: Comic Sans MS">Devoluções</span>. 
{: .text-justify} 

![Figura 1.14: Configuração de uma tabela.]({{ site.url }}{{ site.baseurl
}}/assets/images/TABELA.png){: .align-center}   

{: .image-caption}
*Figura 1.14: Configuração de uma tabela.*
 {: .text-center}
  
![Figura 1.15: Valores obtidos para diversas grandezas do nosso modelo.]({{ site.url }}{{ site.baseurl
}}/assets/images/TABELA_FRAC.png){: .align-center}   

{: .image-caption}
*Figura 1.15: Valores obtidos para diversas grandezas do nosso modelo.*
 {: .text-center}
 
No entanto, estamos com um problema, pois o número de livros deve ser inteiro! Cometemos
um equívoco no modelo e precisamos consertá-lo: precisamos impor que os valores obtidos para
número de livros sejam inteiros. Para isso, vamos retornar às equações que definem os estoques
e usar a função matemática de arredondamento (_Round_), conforme mostrado na Figura 1.16. Ao
clicar nessa função matemática aparecerá o seguinte: _Round(Value)_, no lugar de _Value_ coloque a
equação já criada referente ao fluxo que está sendo arredondado.
{: .text-justify}

![Figura 1.16: Aplicação do arredondamento nas equações.]({{ site.url }}{{ site.baseurl
}}/assets/images/ROUND.png){: .align-center}   

{: .image-caption}
*Figura 1.16: Aplicação do arredondamento nas equações.*
{: .text-center}

Agora sim, rodando essa versão do modelo reproduzimos os valores obtidos pelo bibliotecário. Esse modelo está representado abaixo e disponível no endereço <a href="https://insightmaker.com/insight/198148/
Modelo-da-biblioteca">https://insightmaker.com/insight/198148/
Modelo-da-biblioteca</a>. 
{: .text-justify} 

<p style="text-align: center;"> <iframe width="700" height="500" src="//InsightMaker.com/insight/198148/embed?topBar=1&sideBar=1&zoom=1" 
title="Embedded Insight"></iframe></p>

Como também queremos gerar um gráfico para analisar a mudança dos valores ao longo do
tempo, precisamos clicar novamente em _Add Display_ e escolher a configuração Série Temporal,
adicionar um título ao gráfico em _Title_, escolher as componentes para análise em _Data_, que irão
variar o longo do tempo, e nomear as unidades dos dois eixos de referências (_X-Axis_ e _Y-Axis_).
Agora é só validar a criação clicando em _Apply_. Esses passos estão sintetizados na Figura 1.17 e o gráfico temporal gerado se encontra na Figura 1.18.
{: .text-justify} 

![Figura 1.17: Configuração de um gráfico.]({{ site.url }}{{ site.baseurl
 }}/assets/images/SÉRIETEMPORAL.png){: .align-center}   

{: .image-caption}
*Figura 1.17: Configuração de um gráfico*
 {: .text-center}
  
![Figura 1.18 Gráfico de livros versus tempo.]({{ site.url }}{{ site.baseurl
 }}/assets/images/BIBLIOTECA4.png){: .align-center}   

{: .image-caption}
*Figura 1.18 Gráfico de livros versus tempo.*
 {: .text-center}
 
## Referências
 [4] Asano, C. H. (2009). Cálculo Numérico—Fundamentos e Aplicações (pp. 194-196).<br />
<a href="https://www.ime.usp.br/~asano/LivroNumerico/LivroNumerico.pdf">https://www.ime.usp.br/~asano/LivroNumerico/LivroNumerico.pdf</a>
{: .text-left}
 
 
[<i class="fas fa-arrow-alt-circle-left"></i> Seção 4](https://milenalauschner.github.io/TutorialIM/secao4/){:
.btn .btn--danger} [ Seção 6 <i class="fas fa-arrow-alt-circle-right"></i>](https://milenalauschner.github.io/TutorialIM/secao6/){:
.btn .btn--facebook}
 {: .text-right}
________________________________________________________________________________________________________________________________________________________________________________________________
