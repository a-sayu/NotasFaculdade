# PROVA 1

Tag: #anotacao_geral #SO #SOII

## Índice
1. [[#Conteúdo]]
2. [[#Questão 20 e 21]]

## Conteúdo

É difícil determinar, então vou englobar tudo na primeira prova, da questão 20 à questão 46.

### Questão 20 e 21

Tópicos abordados:
- Problema relacionado a tamanho para a partição
- Maneira de particionar a RAM

Tá, importante mencionar primeiro que existe a partição de **tamanho fixo** e partição de **tamanho variável**.

Partição de tamanho fixo podem ser de *tamanhos iguais* e de *tamanhos diferentes*. Elas são criadas no início das atividades do sistema operacional.

Já as partições de tamanho variável são criadas durante as atividades do sistemas operacionais.

O problema relacionado as partições de tamanho fixo:
- Partição maior que o programa.
- Partição menor que o programa. **Fragmentação Interna**.

O problema relacionado as partições de tamanho variável:
- Após a finalização de um processo, aquele espaço fica, e se tiver sido para um processo pequeno, ele sobra e não é ocupado. **Fragmentação Externa**.

Gerencia da Memória
20: Problemas de Particionamento; Particionamento Variavel
Fragmentação Interna / Particionamento Variavel
21: Quando é feita Partição
Inicio e Durante a Execução
22: Gerenciamento da Memória Secundária
Sistema de Arquivos trabalha com mem. secundária com blocos que podem ser do tamanho de um ou mais setores (arq comp)
39: Qual o nome da falta de divisâo de processos muito pequenos? Atomicidade 

Algo. Escalonamento
23: Como caracterizar algoritmo de escalonamento alternado que permite todas as instruções serem feitas antes de trocar de processo: Justo
24: Como caracterizar algoritmo de escalonamento que fornece tempo igual para todas as instruções: Igualitário
25: Como caracterizar um algoritmo de escalonamento que dá mais tempo por conta de importancia: Prioritário

Contexto
26: Como chamar o conjunto de informações armazenados nos registradores a cada instante sobre a execução de programas: Contexto, utilizado para restaurar processos após uma interrupção.
27: Como processos voltam a ser executaados a partir do ponto em que ele foi interrompido: Através do salvamento e recupereação de contexto.
28: Onde é feito o armazenamento do contexto: Em uma tabela de processos dentro da memória RAM

Compartilhamento de Recursos
29: Forma de controlar o compartilhamento: Mutex
30: Problema em deixar processos do usuários no controle do compartilhamento de recursos: Monopólio
31: Como controlar o compartilhamento: Com uma chamada de sistema
32: Quando deve ser feita a chamada de sistema: Quando o processo precisa de um recurso e finalização do processo com o uso desse recurso.
33: Chamada a Procedimento dentro do codigo
34: O que vc estava fazendo para = interrupcao
36: rotina de tratamento de interrupcao

Driver
37: Sistemas Operacionais precisa de driver para entender recursos
38: Driver é um tradutor

Ciclo de Vida do Processo
40: Ciclo de Vida do processo: Rodando, Bloqueado, Pronto e Concluido

Execução Simultanea
43: Somente se houver mais de um processador

Modo Nucleo e Modo Usuario
45: Programas criticos podem ser usados pelo modo kernel (root) apenas, programas gerais podem ser executados pelo modo usuario (user) em geral
