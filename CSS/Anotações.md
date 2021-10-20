# CSS 



## :id: ID x Classe

ID: é representado pelo símbolo # (hash) e só pode ser utilizado em um elemento.

Classe: é representada por um . (ponto) e pode ser usada em vários elementos.



## :package: Box-model

As margens (margin) são espaçamentos entre elementos;

As bordas (border) circundam o padding e o conteúdo, aparência alterável;

O padding é o espaçamento entre a borda e o conteúdo;

O conteúdo é o que o bloco representa.



## :pencil: list-style-type

Propriedade que altera os marcadores das listas.

É possível customizar com emojis ou imagens, além das opções tradicionais.

`list-style-type: "\1F44D";`

` list-style-image: url("rocket.png"); ` 



## :computer: Flexbox

Método para distribuição de itens e uma interface e recursos de alinhamento.

### :black_medium_small_square: Flex Container

É a tag que envolve os itens (possui itens filhos). É nela que iremos aplicar a propriedade `display: flex `. Transforma todos os seus itens filhos em flex itens. Pode ser feito em qualquer tipo de tag.

Propriedades relacionadas:

- display

- flex-direction 

- flex-wrap

- flex-flow

- justify-content

- align-items

- align-content

  

` display: flex `

Torna a tag um elemento do tipo flex container, e assim automaticamente todos os filhos diretos desta tag tornam-se flex itens.



`flex-direction `

É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no flex container.

São dois eixos: linha (horizontal) e coluna (vertical).

#### Os Eixos

- row (padrão): à direção do texto, esquerda para direita.
- row-reverse: sentido oposto à direção do texto.
- column: ordenação de cima para baixo, em coluna única.
- column-reverse: ordenação inversa, de baixo para cima.



` flex-wrap `

É a propriedade que define se os itens devem ou não quebrar a linha.

Por padrão eles não quebram linhas, isso faz com que os flex items sejam compactados além do limite do conteúdo.

- nowrap: padrão, não permite a quebra de linha.
- wrap: permite a quebra de linha assim que um dos flex items não puder mais ser compactado.
- wrap-reverse: permite a quebra de linha assim que um dos flex items não puder mais ser compactado, porém na direção contrária da linha, acima. 



`flex-flow`

É um atalho para as propriedades flex-direction e flex-wrap.

Porém seu uso não é tão comum, visto que, quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.



` justify-content`

Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção pretendida e tratar da distribuição de espaçamento entre eles.

OBS: caso seus itens estejam ocupando 100% de todo o container, ela não se aplica.

##### As variações

- flex-start: início do container.

- flex-end: final do container.

- center: ao centro do container.

- space-between: cria um espaçamento igual entre os elementos (levando o primeiro item à extrema esquerda e o último à extrema direita).

- space-around: os espaçamentos do meio são duas vezes maiores que o inicial e o final.

  

 `align-items`

Trata do alinhamento dos flex items de acordo com o eixo do container.

O alinhamento é diferente para quando os itens estão em colunas ou linhas.

Permite o alinhamento central no eixo vertical.

Tipos de alinhamento:

- center: alinhamento dos itens ao centro.

- stretch: padrão, e os flex items cresçam igualmente.

- flex-start: alinhamento do itens no início.

- flex-end: alinhamento dos itens no final.

- baseline: alinhamento de acordo com a linha base da tipografia dos itens.

  

 `align-content`

É a propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container.

Precisamos que:

- O container utilize quebra de linhas (`flex-wrap: wrap`)
- A altura do container seja maior que a soma das linhas dos itens.

Tipos de alinhamento:

- center: alinhamento dos itens ao centro
- stretch: é o padrão e os flex items crescem igual
- flex-start: alinhamento dos itens no início
- flex-end: alinhamento dos itens no final
- space-between: cria um espaçamento igual entre os elementos
- space-around: os espaçamentos do meio são 2x maiores que o inicial e final



### :black_medium_small_square: Flex Item

São os elementos filhos diretos do Flex Container. E também podem se tornar Flex Container.

Propriedades relacionadas:

- flex-grow
- flex-basis
- flex-shrink
- flex
- order
- align-self



`flex-grow`

Define a proporcionalidade de crescimento dos itens, respeitando o tamanho de seus conteúdos internos.

OBS: não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container.



`flex-basis`

É a propriedade que estabelece o tamanho inicial do item antes da distribuição de espaço restante dentro dele, usando como base o conteúdo interno disposto.

Valores possíveis:

- auto: caso o item não tenha tamanho, este será proporcional ao conteúdo do item.

- px, %, em, ...: são valores exatos previamente definidos.

- 0 (zero): terá relação com a definição do flex-grow.

  

`flex-shrink`

É a propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item.



`flex`

Esta propriedade é um atalho ou abreviação de escrita para as propriedades: grow, shrink e basis (nessa ordem).



`order`

É a propriedade que lida diretamente com a ordenação dos itens.



`align-self`

É a propriedade que estabelece o alinhamento de modo individual sobre um determinado item.

Valores possíveis:

- auto: valor padrão, irá respeitar a definição de align-items do container.
- flex-start: ao início do container.
- flex-end: ao final do container.
- center: relativo ao center de acordo com o eixo.
- stretch: ocupa todo o espaço relativo.
- baseline: utiliza a linha base da tipografia.

