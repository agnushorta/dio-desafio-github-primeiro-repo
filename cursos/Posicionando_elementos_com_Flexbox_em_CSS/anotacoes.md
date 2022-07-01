# Flex Box

[flxbox MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox), [W3School](https://www.w3schools.com/css/css3_flexbox.asp)

Modelo de layout unidimensional, oferece distribuição de espaço

## Flex Container
É a tag que envolve os itens, é nela que aplicamos a propriedade "display: flex"

### Propriedades relacionadas
- display
- flex-direction
- flex-wrap
- flex-flow
- justify-content
- align-items
- align-content


## Flex Item

São os elementos filhos diretos do Flex Container. E também pose se tornar Flex Container.


![flx-item](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRKQML4QVgTsqFV75YHn0eXWsACisYFv3Jq7A&usqp=CAU)


### Propriedades relacionadas

- flex-grow
- flex-basis
- flex-shrink
- flex
- order
- align-self

### Display: flex;

Torna a tag um elemento do tipo flex container, e assim automanticamente todos os seus filhos diretos desta tag, tornam-se em flex itens. Esta propriedade pode ser aplicada em div, span, section, h1, h2, ..., a

![flx-item](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRKQML4QVgTsqFV75YHn0eXWsACisYFv3Jq7A&usqp=CAU)


### flex-direction

É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no [flex-container](https://developer.mozilla.org/pt-BR/docs/Web/CSS/flex-direction).

![flex-direction](https://res.cloudinary.com/practicaldev/image/fetch/s----O5J3PQ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/4jkkaafn2ef4osrtmhyg.png)

Valores:
- row : (padrão) da direita para a esquerda
- row-reverse : sentido oposto a direção do texto
- column : ordenação de cima para baixo, em coluna única
- column-reverse : ordenação inversa, de baixo para cima

### flex-wrap

É a propriedade [flex-wrap](https://developer.mozilla.org/pt-BR/docs/Web/CSS/flex-wrap) que define se os itens devem ou não quebrar a linha. Por padrão eles não quebram linhas, isso faz com que os flex itens sejam compactados além do limite do conteúdo.

Valores:
- nowrap : é o padrão, não permite a quebra de linha.
- wrap : permite a quebra de linha assim que um dos flex-itens não puder mais ser compactado
- wrap-reverse : permite a quebra de linha assim que um dos flex-itens não puder mais ser compactado, porém na direção contrária da linha, acima.

### flex-flow

A propriedade [flex-flow]() é um atalho para as propriedades **flex-direction** e **flex-warp**.
Porém seu uso não é tão comum, visto que, quando mudamos o *flex-direction* para *column*, mantemos o padrão do flex-wrap que *no-wrap*.

## Justifly Content

Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção pretendida e tratar da distribuição de espaçamento entre eles.

**Obs**: caso seus itens esteja ocupando 100% de todo o container, ele não se aplica

### Variações
 - flex-start: ínicio do container
 - flex-end : final do container
 - center : ao centro do container
 - space-between : cria um espaçamento igual entre os elementos
 - space-around : os espaçamentos do meio são duas vezes maiores que o inicial e final.

 ## Align-items

 Trata do alinhamento dos flex itens de acordo com o eixo do container.
 O alinhamento é diferente para quando os itens estão em colunas ou linhas.
 Permite o alinhamento central no eixo vertical.

 ### Tipos de alinhamentos
 - center: alinhamento dos itens ao centro
 - stretch : padrão, e os flex itens cresçam igualmente
 - flex-start : alinhamento dos itens no início
 - flex-end : alinhamento dos itens no final
 - baseline : alinhamento de acordo com a linha base da tipografia dos itens
 
 ## Align-content

 É a propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container.

 Precisamos que:
    - O conainer utilize quebra de linhas
    - A altura do container seja maior que a soma das linhas dos itens

### Tipos de alinhamentos
 - center: alinhamento dos itens ao centro
 - stretch : padrão, e os flex itens cresçam igualmente
 - flex-start : alinhamento dos itens no início
 - flex-end : alinhamento dos itens no final
 - space-between : cria um espaçamento igual entre os elementos
 - space-around : os espaçamentos do meio são duas vezes maiores que o inicial e final.

