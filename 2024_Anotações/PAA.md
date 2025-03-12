# Anotações Referentes à PAA

Tag: #anotacao_geral #PAA

## 15/10

### Análise de Algoritmos

#### Algoritmo

Procedimentos definidos (seq. de passos) para se obter uma solução para um determinado problema;

Algoritmos são métodos usados para passar soluções para computadores e automatizar soluções;

##### Critérios

Entrada, Saida;

Certeza: Proposta e Instrução é claro;

Finito: Algoritmo termina em um número finito de passos;

Efetividade: Deve ser simplpes para permitir que a pessoa possa realizar testes de papel;

##### Utilidade

1- São fundamentais;

2- Conhecer quais são os melhores algoritmos para cada contexto;

3- Ter a capacidade de projetar novo algoritmos e analisar sua eficiência, conseguindo prever o uso de recursos;

##### Construção de Algoritmos

1- Análise do Problema:

* Entender bem o problema e o que é necessário lidar como entrada e saída

2- Projeto de Algoritmo:

* Projetar o que será implementado, as estruturas de dados mais eficientes, os algoritmos que daram respostas rápidas (tempo de processamento) e pouca ocupação de memória.

3- Implementação:

* Implementar o algoritmo em alguma linguagem de programação.

4- Verificação:

* Dado um conjunto de entradas se ele está produzindo as saídas adequadas ao problema proposto.

##### Eficiencia de Algoritmos

Determinados tipos de problemas podem ser resolvidos de diversas maneiras; e por isso devemos saber qual é o algoritmo mais eficiente.

#### Análisar Algoritmos

Analisar os diversos algoritmos para um mesmo problema = prever os recursos necessários para o algoritmo, e verificar se é viável.

##### Possíveis Técnicas

Experimentação: Executar o algoritmo com diversas entradas e organizações e verificar o resultado e o tempo de processamento, e fazer a comparação;

Análise Assintótica: Análise teórica feita no esboço do algortimo, observando o comportamento do algoritmo, verificando em comportamento em relação ao tamanho da entrada.

* Tempo de Execução: Tempo é precioso;
* Consumo de Memória;

##### Fatores

1- Hardware

* Processador utilizado
* Quantidade de Processadores
* Ciclos por instrução
* Disco (HDD/SSD)
* Memória Prim/Sec
* etc.

2- Software

* SO (kernel, escalonamento, prioridade)
* Linguagem usada
* Compilador usado

3- Natureza de Problema

Dependendo do problema, a organização dos dados pode alterar os resultados, por isso que sempre deve ser mantido as mesmas condições. O conhecimento do algoritmo permite também ver o melhor e o pior caso de execução.

#### Análisar Algoritmos 2

Em uma análise experimental se tem o interesse em determinar o tempo de execução conforme o tamanho da distribuição.

Uma análise por tempo de execução exige:

* Bom Conjunto de Entradas
* Testes Suficientes Executados

Experimentos:

* São úteis e possuem limitações e dificuldades, podendo ser feitos apenas em um número limitado de entradas de teste.
* Geral: qtd de entradas é exponecial.
* Diferentes Algoritmos: É difícil comparar a eficiência de dois algoritmos.

Metodologia:

* Levar em conta todas as entradas possíveis e avaliar a eficiência sem depender de fatores como hardware e software e a necessidade de implementação e execução.

Associar uma função $f(n)$ a cada algoritmo e descrever o crescimento da execução em função da entrada de $n$

## 16/10

### Análise Assintótica

Existem vários componentes que são necessários definir antes de ter uma metodologia de análise de algoritmos baseado em funções matemáticas.

1- Linguagem: Pseudocódigo

* Cuidado com Chamadas Informais: Uma operação/função executada sem descrição do que ocorre.

2- Modelo Computacional: Máquina de acesso aleatório

* Consideramos que algumas/todas operações tem o mesmo custo.
* Acesso direto sem custo de tráfego, escalonamento e etc.

3- Métrica: forma que se calcula a complexidade dos algoritmos.

#### Como Analisar

Contagem de operaçoes para que um algoritmo seja executado, não é no entanto tão detalhado.

Melhor x Pior Caso: Dependem da natureza da entrada de dados.

* Melhor Caso: A entrada que faz a entrada mais eficiente.
* Pior Caso: A entrada que faz a execução menos eficiente.

#### Crescimento das Funções

Lineares : $n$

Quadráticas : $n^2$

O crescimento de uma função qaudrática é maior que o crescimento de uma função linear.

Notação Assintótica: $n$ = $O(n^2)$, essa notação indica o limite superior, ou seja, uma função limitada ao crescimento de outra função, sendo geralmente relacionada ao pior caso de um algoritmo.

O oposto também pode ser dito, podendo indicar o limite inferior, em que uma função está sempre acima de uma outra função.

Notação: $n^2$ = $\Omega(n)$, em que $n$ é igual ou menor que $n^2$, sendo relacionado ao melhor caso de execução de um algoritmo.

#### Classe de Comportamento Assintótico

$O(1)$ ou $O(5)$ ou etc, significam que independente do tamanho de n, as instruções serão executadas um número fixo de vezes.

$O(\log n)$ ocorrem em algoritmos que resolvem um problema transformando em problemas menores, podendo ser considerado menor que uma constante grande.

Ex: Pesquisa Binária

$O(n)$ Um pequeno trabalho é realizao sobre cada elemento de entrada, melhor situação para algoritmos que processam/produzem elementos de entrada/saida. E a cada vez que n dobra de tamamnho o tempo de execução também dobra.

Ex: Pesquisa Sequencial

$O(n \log n)$ ocorrre em algoritmos que resolvem problemas quebrando-os em menores, resolvendo cada um deles independentemente e depois agrupando as soluções.

Ex: Merge Sort

$O(n^2)$ ocorrem quando os itens de dados são processados em pares, se n dobra, o tempo de execução quadruplica. Úteis para problemas relativamente pequenos.

Ex: Selection/Insertion Sort

$O(n^3)$ úteis para resolver problemas relativamente pequenos, em que o tempo de execução é multiplicado por 8.

Ex: Multiplicação de matrizes.

$O(2^n)$ não são úteis do ponto de vista prático, ocorrem no uso de força bruta. Se n dobra, o tempo de execução se eleva ao quadrado.

Ex: Caixeiro Viajante.

$O(n!)$ complexidade exponencial, ocorre também em reposta ao uso de força bruta.

$$\log n > n > n \log n > n^2 > n^3 > n^n > n!$$

## 17/10

### Notação Assintótica Parte 1

Funçoes de mesma ordem são equivalentes; Em geral algoritmos que são assintoticamente mais eficientes serão a melhor escolha para todas as entradas exceto as muito pequenas.

Big O, uma função f domina assintoticamente outra função g / f cresce mais rapidamente que g;

Tempo de execução, T(n) = O(n alguma coisa), existem constantes tais que para valores de n >= a T(n) <= cn alguma coisa.

Smepre lembrar que para testar, precisamos de duas contantes, uma para a função que cresce mais rapidamente (g) e outra para a que é dominada (f) / f $\in$ O(g)

testamos constantes na fórmula de f $<=$ c.g

Podemos desprezar faztores constantes, pois o comportamento assintótico da função continua o mesmo, o mesmo pode ser dito de termos de menor ordem.

### Notação Assintótica Parte 2

$g(n) = O(f(n))$ ou $g(n) \in O(f(n))$ para expressar que a f domina assintoticamente a g;

Outras Notações além de O:

$\Theta$ limite assintoticamente restrito, ou seja f está prensada entre um a mesma função.

$\Omega$ similar a O que define o limite assintotico superior, $\Omega$ define o limite assintótico inferior

$\omega$ se não for assintoticamente restrito, pertence a $\omega$ -> o limite para o infinito é igual a infinito

$o$ se não for assintoticamente restrito, pertence a $o$ -> o limite para infinito é igual a 0

## 18/10

### Recorrências e Teorema Mestre

O objetivo de uma análise é prever os recursos que serão consumidos por um algoritmo.

#### Algoritmos Recursivos

Quando um algoritmo contém chamadas recursivas seu tempo de execução pode ser descrito como uma recorrência.

**Recorrência**: é uma equação que descreve uma função em termos de elementos anteriores da própria equação.

Em chamadas recursivas muitas vezes em que nas chamadas recursivas se reduzem os tamanhos.

Para cada procedimento é associado uma complexidade T(n) desconhecida, onde n mede o tamanho dos argumentos para o procedimento.

#### Teorema Mestre

Resolve recorrências no seguinte formato:

$$T(n) = aT(\frac{n}{b}) + f(n)$$

a >= 1, aT(n/b) representa o numero de chamadas recursivas a cada vez que executa a função, n/b representa em quantas partes se divide o problema (b), e o f(n) representa outros custos envolvidos na chamada recursiva.

1- f(n) é O($n^{\log_b a-\epsilon}$) então $\Theta(n^{\log_b a})$

Falso?

2- f(n) é $\Theta(n^{\log_b a})$ então $\Theta(n^{\log_b a} \log n)$

Falso?

3-f(n) é $\Omega(n^{\log_b a+\epsilon})$ e af(n/b) é menor ou igual a cf(n), então a complexidade é $\Theta(f(n))$

**Não se encaixa no teorema mestre?** Chega-se em somatórios que devem ser resolvidos como séries de por exemplo o matório de 1 até n.

### Análise de Algoritmos de Ordenação

Algoritmos de Ordenação são amplamente usados, sendo importante conhecer os principais e as complexidade deles para saber quando utilizá-los;

Bons exemplos de demonstrar técnicas computacionais;

**Ordenar**: organizar uma sequencia de elementos de modo que os mesmos estabeleçam alguma relação de ordem;

**Ordenar irá facilitar a busca de um elemento?** Nem sempre, pois há vários meios de implementar a ordenação, e dependendo do problema, ordenar para fazer a busca, teria-se que percorrer a lista inteira, usaria a complexidade linear;

Em casos de **muitas consultas**: compensaria uma lista ordenada;

Quando faremos analises, iremos focar nas partes dos algoritmos que ocorrem muito;

Qual a operação dominante?;

#### Baseados em Troca

* BubbleSort : troca-se elementos adjacentes
* QuickSort : ele troca elementos de diferentes partiçoes da lista com base em uma comparação ao pivô

##### BubbleSort

Ele percorre a lista varias vezes, comparando os elementos adjacentes, e alocando os elementos na posição que eles deveriam estar em comparação, em que os numeros iram se mover para próximos de sua posição correta;

Algoritmo Quadrático : Percorreu todo o vetor todas as vezes;

Algoritmo Linear : Percorreu o vetor apenas uma vez;

##### QuickSort

Trocar elementos distantes do vetor, com base em um pivô, o pivô estará na posição correta, que todos os elementos a esquerda serão menores e os da direita maiores que ele;

Complexidade do algoritmo: $n \log n$ em que as partições são quebradas ao meio

Complexidade do Pior Caso: $n^2$

#### Baseados em Inserção

##### Inserção Simples

A inserção simples é um algoritmo que faz uma inserção como se estivesse inserindo ordenado, ele olha para os números e vai inserindo eles na posiçao correta em relaçao ao números que já se tem.

Cria-se uma "lista simulada".

A complexidade de inserção quando já está ordenando é linear: O(n)

O Pior caso é quando está em ordem decrescente, ou seja, um somatório classico, que é uma complexidade quadrática: O($n^2$)

##### Shell Sort

Executa-se a inserção simples em partiçoes do vetor original, criados em diferentes posiçoes do vetor.

Os saltos vão diminuindo conforme estão mais próximas de serem ordenadas.

Teorema 1: O($n^{\frac{3}{2}}$)

Teorema 2: O($n \log n^2$)

#### Baseados em Seleção

Seleciona um elemento e colocar na sua posição correta.

* Seleção Direta
* Heap-sort

##### Selection Sort

Seleciona um elemento e com base nos demais coloca na posição correta. Tanto em seu melhor, quanto no pior tem ordem quadrática.

##### Heap-Sort

Heap sort vai fazer o mesmo encontrando o menor/maior elemento e colocar em sua posição correta. Mas a diferença é que ele vai usar uma estrutura Heap, que implementa uma lista com prioridades, em seu elemento saiz vai ter o maior elemento do vetor, acelerando o processo de seleção.

Heap implementa uma arvore binária quase completa, com ordem $\log n$. Sleeção por meio do rearrajamento do heap que tem custo de log n.

A complexidade do Heap-Sort é $\Theta(n \log n)$

#### Baseado em Intercalação

##### Merge-Sort

Fazer a divisão e conquista, ou seja, dividir o array até o menor caso, que é simples de ordenar, e vai-se compondo a lista na etapa de conquista, reposicionando os elementos de forma ordenada.

A complexidade do Merge Sort é $n \log n$, se voce tiver um array mt grande ele vai quequisitar o dobro de memória desse array
