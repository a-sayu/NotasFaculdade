# Aula de Projeto e Análise de Algoritmos

Tags: #PAA

## Programação Dinâmica

É uma estratégia muito interessante que não está voltada para a programação em si, mas em estratégias de solução. Tendo como propósito reduzir custos de outras estratégias para que a complexidade caia.

Um exemplo Simples:

* Fibonacci
Há uma sobreposição de problemas, sendo necessário resolver a mesma coisa para o mesmo problema.

Podemos armazenar em uma tabela os mesmos problemas, de forma a reduzir cálculos e não re-calcular

O que observaos:

A quebra em subproblemas e a identificação de um sub-estrutura ótima, reaproveitando somas anteriores.

Diferença entre Divisão e Conquista com Programação Dinâmica

Os dois utilizam de quebra em subproblemas, mas enquanto o divisão e conquista utiliza todos os subproblemas, a programação dinâmica utiliza apenas as subestruturas ótimas.

### Problema 1: Uma mochila booleana com capacidade C, e com N itens disponíveis (cada um com um peso W e um valor V)

Queremos selecionar itens de forma que não exceda a capacidade da mochila e se tem o valor máximo agregado.

Suponha que usemos um algoritmo guloso, não selecionaremos a melhor solução, o máximo global, nem mesmo com o uso de proporção de valor/peso;

Combinatório $O(2^n)$;

### Exemplo 2: Mochila Booleana C=6, N=3

Primeiro ponto para quebrar, se resolveria o ponto de capacidade de mochila a cada capacidade, além de considerar a quantidade de itens considerados para serem resolvidos em cada capacidade.

1 : Apenas um item a ser considerado

* Item A 50/4 : 1:0{-} 2:0{-} 3:0 4:1{A} 5:1{A} 6:1{A}
* Item B 40/2 : 1:0{-} 2:1{B} 3:1{B} 4:1{A} 5:{A} 6:{A,B} // Apenas etapas sem solução recebem o item B, e para as que tem, se pergunta a melhor opção, na op 4, compensa trocar ou adicionar um de valor 50 com um de valor 40? Não. Ele considera as etapas anteriores, na op 6 ele identificou que somando a op 4 com o novo item, o peso não é ultrapassado e o valor supera o valor anterior.
* Item C 45/3 : 1:0{-} 2:1{B} 3:1{C} 4:1{A} 5:{B,C} 6:{A,B}

Portanto ao final, ele irá falar que a união do item A com o item B chega na melhor solução. Saindo de algo exponencial, para percorrer uma matriz de complexidade de num Elemento pela cap Mochila (NxC).
