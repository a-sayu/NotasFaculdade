# Aula de Estrutura de Dados II

## Grafos

Como calcular o grau, que é número de vizinhos de um vértice.

### Popularidade

Aquele que tem o maior grau.

### Grafos Dirigidos - Dígrafos

As vértices são conectados de forma dirigida indicando início e fim

### Numero de Arestas de um Grafo

Quantas conexões/arestas se tem um gráfico com $n$ vértices:

$$\frac{n(n-1)}{2} = O(n^2)$$

### Grafos Esparsos

Um grafo pode ter o número máximo de arestas definidas pela fórmula, mas pode ter bem menos. Um grafo é esparso se ele possuir "poucas" arestas, menos que o definido pela fórmula.

### Lista de Adjacência

Uma lista ligada para cada vértice, armazenando quem são os vizinhos do vértice

* Se há um grafo pouco preenchido, pois ocupa muito espaço de memória.
