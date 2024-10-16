# Anotações Referentes à PAA

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

### Notação Assintótica Parte 1

### Notação Assintótica Parte 2

## 17/10

### Análise de Algoritmos Recursivos

### Análise de Algoritmos de Ordenação

## Nota

;
