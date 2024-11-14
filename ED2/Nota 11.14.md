# Grafos

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
