# Aula de Projeto e Análise de Algoritmos

Tag: #2_Ano #PAA

## Força Bruta

Geralmente é a primeira solução pensada, em observação:

* Selection Sort
* Bubble Sort
* Busca Sequencial
* Verificar Casamento de Strings
* Multiplicação de Matrizes

Realmente, alguns roblemas não possuem uma solução algorítmica eficiente, sendo necessário implementar a força bruta.

Uma estratégia para isso: Heurística e afins, mas que não chegam em soluções ótimas, mas em soluções aproximadas.

**Exemplo:** Caixeiro Viajante - Passar por cada cidade uma única vez e voltar a origem, considerando o circuito de custo mínimo, em que não se tem a resuloção ótima ainda.

Ciclo Amiltaniano - Ciclo sem repetição de vértices - neste caso, que a soma das arestas é o menor possível.

Neste exemplo, há um caso de perguntações, em que é necessário vários testes, resultado em uma complexidade exponencial.

Não faz sentido ir à um caminho que não existe/não há conexão.

### Tentativa e Erro

* Backtracking: problemas de encontrar uma solução/decisão.
* Branch-and-bound: além de solução há a necessidade da melhor solução.

Nesta estratégia de evolução de estados podemos fazer podas na árvores de busca, eliminando coisas que influenciam na velocidade da resposta.

### Backtracking

Deriva-se até o estado, e se não chegar na solução, retorna ao estado anterior continuando a busca em derivação pela solução.

#### Problema das N-Rainhas

Você tem um tabureiro de xadrez nxn, e é necessário posicionar as **n** rainhas de forma que elas não se ataquem.

### Branch-and-Bound

Quando-se tem um problema de que se quer a melhor solução, sendo necessário varrer quase tudo para achar a solução ótima. Ele poda também baseado em custo, verificando se o custo atual é ainda inferior ao custo deuma solução anterior.

#### Problema de Associação de Tarefas

Você tem pessoas e tarefas para associar essas pessoas, portanto alocando as pessoas para minimizar os custos de alocação de pessoas.
