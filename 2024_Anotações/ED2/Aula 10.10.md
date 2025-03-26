# Aula de Estrutura de Dados II

Tag: #2_Ano #ED2

Nota: Realizar revisão do Slide de Grafos Parte 2 até o slide 35 (pág. 6)

## Percurso em Grafos

### Caminho em Grafos

Um caminho de um ponto $s$ para $t$ em um grafo é:

* Uma sequência sem repetição de vértices vizinhos

### Componentes Conexas

### Existe caminho entre s e t?

#### Exemplo - Existe caminho de 0 até 15?

Ele pega um caminho conectado ao 0 e vai em seguinte, marcando como visitado, e se não há mais ninguém, ele retorna, perguntando se há arestas que não foram visitados.

#### Implementação Matriz de Adjacência

Implementação com matriz de adjacências.

[[Existe_Caminho.png]]

#### Implementação Componentes Conexas

Implementação com listas de adjacência.
