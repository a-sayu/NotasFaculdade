
Tag: #3_Ano #SO #SOII 

Questão 25.

Quando começamos a falar de sistemas operacionais, jogamos um jogo de administração de uma empresa, só que a invés de administrar uma empresa, o sistema operacional administra um computador, organizando os recursos do computar, os processos.

Em um primeiro momento ligamos ao programa os processos, mas em sistemas operacionais, um processos são um conjunto de atividades, envolvendo não so um programa, mas um conjunto de informações necessárias para o programa, os dados de entrada, resultados e o estado em que o processo se encontra no determinado momento, além de que processos também passam por um ciclo de vida.

Então tudo que tem haver com um processo, com excessão dos recursos fisicos, a não ser a administração dos recursos físicos, faz parte de um processo.

Escalonamento existem de vários tipos, mas o que estudaremos sera o de processador

Round Robin: É o mais comum atribuido ao processador, em que se tem uma fila, mostrando o processo atual e os seguintes processos que irão ter acesso a um quantum do processador, que é uma fatia de tempo do processador. Ele não implementa prioridade

Filas Multiplas: Tem várias filas separadas por prioridades, em que as prioridades superiores são executadas primeiro, indo de cima para baixo, exemplo, tem 3 filas. Fila a, b e c, a execução iria: a1, a2, a3, b1, a1, a2, a3, b2, a1, a2, a3, b3, a1, a2, a3, c1, a1, a2, a3, b1... Em diante.

Questão 27.
A sua equipe chegou à conclusão de que ocorre escalonamento entre os processos de usuário responsáveis pelos dois tipos de movimentos distintos efetuados pelo braço robótico. Problema: você precisa explicar como cada processo consegue voltar a ser executado exatamente a partir do ponto em que ele foi interrompido quando o seu quantum expirou.

Minha Resposta: Pois quando o quantum do processo terminou, o contexto/estado salvo foi recuperado.