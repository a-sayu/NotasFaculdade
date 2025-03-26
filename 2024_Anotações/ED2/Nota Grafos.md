# Grafos

Tag: #2_Ano #ED2
## O que é um Grafo?

É um conjunto de **vértices** ligados entre si por **arestas**

**Como representar matemáticamente um Grafo:**

É um par ordenado de conjuntos: (V, E)

* **V** sendo o conjunto de vértices/todos os pontos do grafo.  
Exemplo: {1, 2, 3, 4, 5}
* **U** sendo o conjunto de arestas/ligações entre os pontos, arestas são representadas com um mini conjunto com as duas arestas ligadas.  
Exemplo de Aresta: {a, b}, a!= b, sendo este um conjunto único  
Exemplo de Conjunto de Arestas: {{a,b},{a,d},{b,c},{c,e},{e,d}}

**Adjacência:** é quando há uma conexão com um outro vértice diferente do observado, chamado de vizinho, e um conjunto de vizinhos formam uma vizinhança.

## Matriz de Adjacências

Um grafo pode ser representado por uma matriz de adjacências, com n colunas e n linhas (nxn).

* 'n' representando a quantidade de vértices
* Sendo os vértices enumerados de 0 à n-1.
* E dentro dessa matriz, onde os dois vértices "se encontram", se houver um **1**, significa que eles são vizinhos, e se houver um **0**, eles não são.

OBS: Código Implementado em Repositório (Slides 7-10)

## 11.15

## Amigos x Seguidores

Amigos são aqueles que tanto de um lado quanto do outro são vizinhos.

Portanto existe uma aresta entre um 'u' e um 'v'.

Seguidores são aqueles que apenas de um lago são "vizinhos".

Portanto existe um arco em que 'u' aponta para 'v'

## Grafos Dirigidos

Um grafo com um conjunto de vértices, conectados por um conjunto de arcos, que são arestas indicando o seu inicio e o seu fim.

**u** é origem.  
**v** é destino.  

Uma matriz de adjacencia pode ser usada para representar um digrafo.

## Arestas

Um grafo com n vértices pode ter $\frac{n.(n-1)}{2}$ arestas.

Entretanto, sabemos que nem todos esses vértices estão conectados, além de que para grafos enormes, não caberiam isso tudo na memória.

## Grafo Esparso

Um grafo esparso é aquele que tem "poucas" arestas, no caso bem menos que o número máximo.

Exemplos:

* Grafos com um Grau Máximo $\frac{d.n}{2}$
* Grafos com $O(n\log n)$ arestas

**!**: Grafos que ainda são de ordem $n^2$ não são esparsos.

## Listas de Adjacência

Grafos podem ser representados por listas de asjacência, sendo por exemplo um vetor que possuem uma lista encadeada para cada vértice (posição no vetor), que armazena quais são os vizinhos do vértice.
