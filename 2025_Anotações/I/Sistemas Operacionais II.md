# PROVA 1

Tag: #anotacao_geral #SO #SOII

## Índice
1. [[#Conteúdo]]
2. [[#Questão 20, 21 e 22]]
3. [[#Questão 23, 24 e 25]]
4. [[#Questão 26, 27 e 28]]
5. [[#Questão 29, 30, 31, 32 e 33]]
6. [[#Questão 34, 35(47), 36 e 39]]
7. [[#Questão 37 e 38]]
8. [[#Questão 40]]
9. [[#Questão 43]]
10. [[#Questão 45]]
11. [[#Questão 46]]

## Conteúdo

É difícil determinar, então vou englobar tudo na primeira prova, da questão 20 à questão 46.

### Questão 20, 21 e 22

Tópicos abordados:
- Particionamento
- Maneira de particionar a RAM
- Momento de particionamento da RAM
- Problema relacionado a tamanho para a partição
- Particionamento na Memória Secundária

Tá, importante mencionar primeiro que existe a partição de **tamanho fixo** e partição de **tamanho variável**.

Partição de tamanho fixo podem ser de *tamanhos iguais* e de *tamanhos diferentes*. Elas são criadas no início das atividades do sistema operacional.

Já as partições de tamanho variável são criadas durante as atividades do sistemas operacionais.

> *Importante notar que um sistema operacional apenas lida com um tipo das possíveis formas de partição.*

O problema relacionado as partições de tamanho fixo:
- Partição maior que o programa.
- Partição menor que o programa. **Fragmentação Interna**.

O problema relacionado as partições de tamanho variável:
- Após a finalização de um processo, aquele espaço fica, e se tiver sido para um processo pequeno, ele sobra e não é ocupado. **Fragmentação Externa**.

O sistema operacional também gerencia a memória secundária com o sistema de arquivos, organizando em blocos que podem ser do tamanho de um a mais setores (*arquitetura de computadores*).

### Questão 23, 24 e 25

Tópicos abordados:
- Características do algoritmo de escalonamento.

...

### Questão 26, 27 e 28

Tópicos abordados:
- Contexto
- Tabela de Processos

...

### Questão 29, 30, 31, 32 e 33

Tópicos abordados:
- Controle de compartilhamento de recursos
- Problemas de responsabilizar usuários no controle de compartilhamento
- Mecanismos de sincronização
- Mutex
- Chamada do Sistema e quando ocorrem
- Chamada à procedimento

### Questão 34, 35(47), 36 e 39

Tópicos abordados:
- O que é interrupção
- Como o sistema operacional lida com interrupções
- Quantos vetores de interrupção o sistema operacional deve possuir
- O que é vetor de interrupção
- Porque um processo pode não ser interrompido?

...

### Questão 37 e 38

Tópicos abordados:
- O sistema sabe lidar diretamente com qualquer tipo de periférico?
- O que ele precisa ter para lidar?
- O que é um driver?

...

### Questão 40

Tópicos abordados:
- Ciclo de vida dos processos

...

### Questão 43

Tópicos abordados:
- Execução simultânea de processos

...

### Questão 45

Tópicos abordados:
- Modo Núcleo e Modo Usuário

...

### Questão 46

Tópicos abordados:
- O que a MMU faz?

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
>>>>>>> origin/main
