# Aula de Projetos e Análise de Algoritmos

Tag: #2_Ano #PAA

## Algoritmos Gulosos

A ideia é que ele tente chegar em uma solução sem nunca voltar atrás, em que na etapa atual a busca pela solução, ele vai optar pelo item mais "apetitoso"/favorável.

Alguns algoritmos podem ser pensados que são facilmente resolvidos por um algoritmo guloso, mas não chegam num caso ótimo.

É uma estratégia de complexidade baixa, rápido, mas que não chega na solução ótima.

### Exemplo: Problema do Troco

Dada uma quantidade de troco que deve ser devolvida, se espera a menor quantidade de moedas possível.

A cada iteração, se eu consigo utilizar a moeda de maior valor, se usa ela. Uma vez chegado no valor desejado, essa seria a melhor "escolha" de conjunto de moedas.

Algoritmos gulosos são complicados de validar.

Ótimo Local x Ótimo Global

A quantidade de moedas é pequena, mas não é 'A' melhor.

## Árvore Geradora Mínima

Tem-se um grafo de valor A, mas você quer um subconjunto conexo dele, em que o somatorio do valor das arestas desse novo grafo seja o mínimo possível, sem forma ciclos. Qualquer outra arvore gerada não terá um valor menor que esse.

Existem dois algoritmos de arvore geradora mínima gulosa.

### Como eu chego na certeza que é uma árvore geradora mínima?

### PRIM

Corte em grafos, em que se simula cortes para separar o grafo em dois, um que está no corte e outro que não está.

Arestas que cruzam o corte: que conectam vertices de um conjunto e o outro.

Aresta leve: dentre as arestas que cruzam o corte, qual que é a de menor valor?

### KRUSKAL

Ainda mais direto que o PRIM, em que se tem um grafo, que se cria conjuntos disjuntos, em que cada vertice é representado por um conjunto, ele vai ordenar pelo peso das arestas.

Uma vez ordenado, ele vai percorrer a lista adicionando elas na solução.

É necessário ter cuidado em se forma ciclos, portanto sempre checando.

A diferença é que se formaram florestas antes de formar arvores.

#### Como ele sabe se forma ciclo ou não?

Ele observa se o vertice X e Y estão em um mesmo conjunto.

União de Conjuntos Disjuntos > O maior problema.

**Sempre chega num ótimo global.**

Em torno de $O(n \log n)$

## Para finalizar

Existe uma estratégia já vista, mas que está mais batida

## Divisão e Conquista

Dividir o problema em partes menores, de modo que se resolva essas partes até chegar na solução globalmente. Merge, Quick, utilizam essa estratégia, chegando na solução final.

Em um livro, busca binária seria um Diminuir para Conquistar. Ele quebra o problema em partes, sendo lidados x vezes, tendo um custo adicional da "conquista".
