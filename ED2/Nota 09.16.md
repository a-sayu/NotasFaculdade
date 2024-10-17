# Estudando para Estrutura de dados II

As estruturas estudadas anteriormente estudadas como Árvore Binária de Busca, Árvore AVL, Árvores Rubro-Negra são adequadas para a memória primária, onde o tempo de acesso é rápido, mas na memória secundária o desempenho se torna ínfimo.

Algoritmos rápidos para uma memória secundária são regidos pela leitura e escrita no disco, e a Árvore B é uma estrutura que reduz o número de acessos e o tempo gasto em operações (busca, inserção e remoção).

Um disco é dividido em páginas/blocos de tamanho fixo.

Para a aplicação de uma Árvore B, a quantidade de dados que precisam ser acessados não cabem na memória primária, e portanto cada nó tem o tamanho de uma página do disco, que facilita o acesso.
