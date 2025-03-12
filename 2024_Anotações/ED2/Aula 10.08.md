# Aula de Estrutura de Dados II

Tag: #ED2

Vimos na última aula o algoritmo de recomendação.

O grafo não precisa ser unidirecional, pode ser bidirecional também.

* O que é essa matriz de confusão que o professor fica confundindo?

Quantas arestas máximas tem um gráfico?
Existe outros modos de representar pela matriz de adjacência.

Lista de Adjacência.

Quando eu uso Matriz e Lista? Lista quando se tem mais posições vazias e Matriz quando se há mais posições preenchidas.

```c
typedef struct No {
int v;
struct No *prox;
} No;

typedef No *p_no;

typedef struct {
p_no *adjacencia;
int n;
} Grafo;

typedef Grafo *p_grafo;

p_grafo criar_grafo(int n) // Número de vértices

void destroi_grafo(p_grafo g);

void insere_aresta(p_grafo g, int u, int v);

void remove_aresta(p_grafo g, int u, int v);

int tem_aresta(p_grafo g, int u, int v);

void imprime_arestas(p_grafo g);
```

## Inicialização

```c
p_grafo criar_grafo(int n) {
int i;
p_grafo g = malloc(sizeof(Grafo));
g->n = n;
g->adjacencia = malloc(n * sizeof(p_no));
for (i = 0; i < n; i++)
g->adjacencia[i] = NULL;
return g;
}
```

```c
void libera_lista(p_no lista) {
if (lista != NULL) {
libera_lista(lista ->prox);
free(lista);
}
}
```

Ele libera uma lista por vez.

## Destruição

```c
void destroi_grafo(p_grafo g) {
int i;
for (i = 0; i < g->n; i++)
libera_lista(g->adjacencia[i]);
free(g->adjacencia);
free(g);
} 
```

### Como estrutura de dados se integra com banco de dados?

Arvore B, Hash... Quebrar em arquivos menores. Spark = poderia ter um arquivo com 1 milhao de clientes, o spark pega esse arquivo e quebra em diversos arquivos pequenos, e para buscar ele pega varios computadores para ler pedacinhos de arquivo. Na hora em que se quebra os caras, é necessário saber onde se quebra eles. Hash evita vazios e sequenciais.

Fila, Lista é utilizado mais em memória. Uma busca em um ponto 3d, uma busca espacial de cidades em até 100km, procurando todas os pontos relacionados próximos deste ponto, calculando a distancia até o ponto e pegando apenas aquelas que estão numa distancia determinada.

Bancos SIG (Sistema de Informação Geográfica), muito importante utilizar árvores

## Inserção

```c
p_no insere_na_lista(p_no lista , int v) {
p_no novo = malloc(sizeof(No));
novo ->v = v;
novo ->prox = lista;
return novo;
}
```

```c
void insere_aresta(p_grafo g, int u, int v) {
g->adjacencia[v] = insere_na_lista(g->adjacencia[v], u);
g->adjacencia[u] = insere_na_lista(g->adjacencia[u], v);
}
```

Inserir um cara em uma lista específica.

1 -> 2 -> 4 --
2 -> 1 -> 4 -> 3 --
3 -> 2 --
4 -> 1 -> 2 --

Cria uma caixinha
( | )
Adiciona na caixinha o novo no
( 3 | )
Aponta para a sequencia que viria (a adjacencia do grafo desse no)
(3 | ->1 -> 2--)
A nova adjacência agora é essa caixinha
4 -> (3 | -> 1 -> 2 --)

## Remoção

```c
p_no remove_da_lista(p_no lista , int v) {
p_no proximo;
if (lista == NULL)
return NULL;
else if (lista ->v == v) {
proximo = lista ->prox;
free(lista);
return proximo;
} else {
lista ->prox = remove_da_lista(lista ->prox , v);
return lista;
}
}
```

```c
void remove_aresta(p_grafo g, int u, int v) {
g->adjacencia[u] = remove_da_lista(g->adjacencia[u], v);
g->adjacencia[v] = remove_da_lista(g->adjacencia[v], u);
}
```

## Verificar se há, e Impressão

```c
int tem_aresta(p_grafo g, int u, int v) {
p_no t;
for (t = g->adjacencia[u]; t != NULL; t = t->prox)
if (t->v == v)
return 1;
return 0;
}

void imprime_arestas(p_grafo g) {
int u;
p_no t;
for (u = 0; u < g->n; u++)
for (t = g->adjacencia[u]; t != NULL; t = t->prox)
printf("{%d,%d}\n", u, t->v);
}
```
