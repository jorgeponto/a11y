voltar ao [sumário](README.md)

<h1>1. Menus de navegação</h1>

conteúdo do capítulo:

- [Introdução](#Introdução)
- [Racional do ponto de verificação](#racional-do-ponto-de-verificação)
- [Requisitos WCAG 2.1 aplicáveis](#requisitos-wcag-21-aplicáveis)
- [Avaliação dos requisitos constantes na Checklist "10 aspetos críticos de acessibilidade funcional"](#avaliação-dos-requisitos-constantes-na-checklist-10-aspetos-cr%C3%ADticos-de-acessibilidade-funcional)
  - [Procedimento de teste](#Procedimento-de-teste)
  - [Ferramentas de validação](#ferramentas-de-validação)
- [Checklist "10 aspetos críticos de acessibilidade funcional"](#checklist-10-aspetos-cr%C3%ADticos-de-acessibilidade-funcional)

## Introdução

É comum num sítio Web existirem vários menus de navegação. No presente capítulo vamos apenas debruçarmo-nos sobre o menu que constitui no sítio Web o menu principal de navegação. Geralmente, este menu está presente em todas as páginas do sítio Web, posicionado no topo das páginas e apresenta as suas diversas opções de forma horizontal, vertical ou, até mesmo, em painéis. Na verdade, a forma visual como se apresenta é pouco relevante para a verificação dos requisitos aqui presentes.

O menu principal de um sítio Web é, por regra, o mecanismo de entrada, ou passagem, para as partes mais importantes do sítio Web. Não conseguir aceder, entender ou manusear o menu principal é uma barreira à entrada e à utilização do sítio Web. Ele é a génese do princípio do descalabro e da insatisfação que leva o utilizador a procurar uma estratégia alternativa de navegação - um motor de pesquisa no sítio, por exemplo - ou mesmo, a procurar soluções fora do sítio Web.

## Racional do ponto de verificação

Um menu é, em termos estruturais, uma lista de opções. Quando o número de elementos a disponibilizar é grande, por questões de facilidade de leitura e maquetização espacial, organizam-se esses mesmos elementos em opções e subopões - na [Checklist "Conteúdo" do selo de Usabilidade e Acessibilidade recomenda-se mesmo que o menu e os submenus não tenham mais do que 9 opções](#).

Em acessibilidade, e porque estes elementos são relevantes para as tecnologias de apoio que, muitas vezes, fazem a intermediação da leitura para o utilizador final, há dois parâmetros num menu que é importante preservar: 

- a noção de lista de opções e;
- o facto de as opções e as subopções terem que ser alcançadas por utilizadores que usem rato (ou qualquer outro dispositivo apontador) ou teclado (ou qualquer outra tecnologia que se comporte como o teclado).

A preservação da semântica - "lista de opções" - é, por exemplo em HTML, alcançada usando elementos de HTML próprios para marcar listas. É o caso do exemplo que se apresenta abaixo:

```html
<ul>
   <li>início</li>
   <li>Recursos
      <ul>
         <li>Tutorial sobre imagens</li>
         <li>Tutorial sobre formulários</li>
      </ul>
    </li>
    <li>Blogue</li>
</ul>
```
Figura: Lista de opções do tipo UL - <em lang="en">unorder list</em> (lista não ordenada de itens).

A representação visual, horizontal ou vertical, com as subopções abertas ou fechadas, deve ser controlada com o uso de CSS (folhas de estilo em cascata).

Alcançar as opções e as subopções usando apenas um teclado ou usando apenas um rato está relacionado com o uso de manipulares de eventos de javascript independentes (do tipo `onfocus` e `onblur`) ou então redundantes, próprios para o rato (tipo `onmouseover`) ou para o teclado (`onkeypress`).

## Requisitos a cumprir

### 1.1 O menu de navegação está estruturado como uma lista de opções e subopções

Para que possa ser bem interpretado pelas tecnologias de apoio, os menus e submenus devem estar estruturados com elementos HTML nativos, do tipo `<ul><li>(...)`, ou com a semântica e o estado dos elementos identificados com técnicas de ARIA.

### 1.2 As opções e subopções do menu são selecionáveis com rato e com teclado

Deve ser possível percorrer a estrutura de navegação quer com um dispositivo apontador quer com o teclado.

### 1.3 As imagens-link, quando usadas para construir mecanismos de navegação, têm o correspondente equivalente alternativo em texto

Quando as imagens-link dispõem de um equivalente alternativo em texto, também designado tecnicamente de nome acessível, permitem que os mecanismos de navegação sejam utilizados de múltiplas formas. Por exemplo, para quem não vê podem transformar-se em texto. Para quem não consegue controlar um rato ou  teclado podem ser ativados através de reconhecimento de fala.


## Avaliação

### Procedimento de teste

*Analisar a estrutura do menu*

A estrutura do menu poderá ser analisada desativando as folhas de estilo. Por exemplo, no caso do menu cujo código apresentámos na figura atrás obteríamos algo como:

<blockquote>
  <ul>
    <li>início</li>
    <li>Recursos
      <ul>
        <li>Tutorial sobre imagens</li>
        <li>Tutorial sobre formulários</li>
      </ul>
    </li>
    <li>Blogue</li>
  </ul>
</blockquote>
Figura: exemplo de uma lista encadeada de opções com o estilo definido por <span lang="en">**Tim Berners-Lee**</span> no início dos anos 90.

*Acesso às opções e subopções usando apenas o rato ou usando apenas o teclado*

Uma das formas mais fáceis para testar este critério é "estacionar" o rato e, usando apenas o teclado, tentar navegar pelas opções e subopções pressionando na tecla `TAB` para andar para a frente e `Shift-TAB` para andar para trás.

Pode-se fazer o mesmo mas desta vez usando apenas o rato. Será pouco provável que o rato esteja condicionado de aceder a alguma opção ou subopção mas poderá acontecer.

*Imagens-link*

Desative as imagens (usando por exemplo uma barra de ferramentas de acessibilidade para o browser) e verifique se no lugar das imagens aparecem alternativas equivalentes em texto. Também pode efetuar a leitura recorrendo a um leitor de ecrã.


### Ferramentas de teste

Para analisar a estrutura pode-se usar uma "Barra de Ferramentas de Acessibilidade" para instalar no navegador Web. Geralmente estas barras de ferramentas dispõem de opções para retirar os estilos da página.

Para análise das imagens-link nas barras de ferramentas também é possível solicitar uma análise ao texto alternativo existente nas imagens.

Outra possibilidade é usar um leitor de ecrã como é o caso do NVDA (opensource e disponível gratuitamente), ChromeVox existente no navegador Web da Google, o Chrome.

## Checklist

<table>
<caption>O que verificar no <strong>menu de navegação principal</strong></caption>
 <tr>
  <th align="left">verifique se:</th>
  <th>sim</th>
  <th>não</th>
  <th><abbr title="não aplicável">n.a</abbr></th>
 </tr>
 <tr>
  <td>a) o menu de navegação está marcado como uma lista do tipo <code>&lt;ul&gt;</code>?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>b) é possível navegar com rato e com teclado?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td>c) as imagens-link, caso existam no menu, estão corretamente legendadas?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
</table>

voltar ao [sumário](README.md)

# 1. Menu de navegação principal

O menu de navegação principal é como a porta de entrada de uma casa. Para entrar dentro de casa é preciso alcançar a porta e passar a porta. Se não o conseguirmos fazer, será impossível usufruir da casa. Num sítio Web, podemos muito bem usar a porta como metáfora para representar o menu principal. Se o utilizador não encontrar o menu principal ou não conseguir navegar pelas suas opções e subopções então nunca irá conseguir usufruir da informação ou dos serviços disponíveis nesse sítio.

Numa página Web, um menu é, em termos estruturais, uma lista de opções. Quando o número de elementos a disponibilizar é grande, por questões de facilidade de leitura e maquetização espacial, organizam-se esses mesmos elementos em opções e subopões. Através do sentido da visão, a perceção desta organização é, quase sempre, simples, lógica e evidente - os designers gráficos são, em 99% dos casos, muito bons a transmitir a organização de um menu a quem faz uso da visão. A dificuldade surge quando o menu tem de ser percecionado por outra via que não através da imagem - por exemplo, como representar um menu no caso de uma pessoa cega?

Quase sempre, em acessibilidade Web, a resposta a esta e outras perguntas de representar algo de uma outra forma, para ir ao encontro das capacidades de um utilizador com determinadas limitações funcionais, é dada pela conjugação de duas tecnologias: as tecnologias de acesso e as tecnologias de marcação do conteúdo digital. Por exemplo, no caso de uma pessoa cega, quando nos referimos a tecnologias de acesso estamos a falar do navegador Web e do leitor de ecrã.

<table>
<caption>Lista de verificação para <strong>menus de navegação</strong></caption>
 <tr>
  <th style="width:70%; text-align:left;">verifique se:</th>
  <th style="width:10%">sim</th>
  <th style="width:10%">não</th>
  <th style="width:10%"><abbr title="não aplicável">n.a</abbr></th>
 </tr>
 <tr>
  <td style="align:right">a) o menu de navegação está marcado como uma lista do tipo <code>&lt;ul&gt;</code>?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td style="align:right">b) é possível navegar com rato e com teclado?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
 <tr>
  <td style="align:right">c) as imagens-link, caso existam no menu, estão corretamente legendadas?</td>
  <td></td>
  <td></td>
  <td></td>
 </tr>
</table>
