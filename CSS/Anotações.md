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

### Flex Container

É a tag que envolve os itens (possui itens filhos). É nela que iremos aplicar a propriedade `display: flex `. Transforma todos os seus itens filhos em flex itens. Pode ser feito em qualquer tipo de tag.

Propriedades relacionadas:

- display
- flex-direction 
- flex-wrap
- flex-flow
- justify-content
- align-items
- align-content



### Flex Item

São os elementos filhos diretos do Flex Container. E também podem se tornar Flex Container.

Propriedades relacionadas:

- flex-grow
- flex-basis
- flex-shrink
- flex
- order
- align-self