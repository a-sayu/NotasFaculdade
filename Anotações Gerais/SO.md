# PROVA 1 : Sistemas Operacionais

Tag: #anotacao_geral #SO

## Conteúdo

**Suposição, não confirmada?*

Questões 1 à 14

## Anotações de Revisão

**Questão 1**:

Contexto: A FCT designou a sua equipe para desenvolver um novo sistema operacional "a partir do zero" para certo sistema de computação.

Problema: Você deve identificar o que vocês precisam saber ANTES de começar o projeto do sistema operacional, ou seja, qual conhecimento é essencial ANTES que o projeto possa ser iniciado.

Resposta: Todas as alternativas anteriores: Fabricante, Velocidade, Marca e Modelo do sistema de computação e Recursos disponíveis e características gerais dos programas de usuários  

**Questão 2**:

Problema: Apesar de não ver todo hardware que compõe o sistema, você deve ser capaz de deduzir quais são os quatro principais recursos (em hardware) que estão à disposição do sistema.  

Resposta: Processador, RAM, periféricos e HD/SSD  

**Questão 3**:

Problema: Use o seu ponto de vista como desenvolvedor de arquiteturas de computadores para classificar o braço robótico quanto ao tipo de hardware que ele é, de acordo com a função que ele exerce dentro do sistema computacional apresentado pela nossa empresa.  

Resposta: Dispositivo Periférico  

**Questão 4**:

Contexto: Você foi chamado pela nossa empresa para participar desta reunião em que um sistema de computação em operação está sendo apresentado. O motivo pelo qual você está aqui é que a nossa empresa acredita na sua capacidade para tentar desvendar os segredos que existem por trás desse sistema computacional. Tudo que se sabe até agora sobre esse sistema é que ele é composto por um computador, um braço robótico, um sistema operacional e dois programas de usuário, sendo que cada programa de usuário leva dez minutos para terminar a sua execução por completo. Após presenciar o funcionamento desse sistema, a empresa espera que você seja capaz de solucionar os problemas que serão levantados por ela nas questões que serão apresentadas a você durante esta reunião.  

Problema: Agora que a sua equipe já conhece os recursos disponíveis na FCTarc13 e as características dos programas de usuários, use este contexto para elaborar uma justificativa para a sua equipe sobre o motivo técnico pelo qual vocês irão desenvolver um sistema operacional  

Resposta: Para que programas de usuário sejam executados dando a impressão de execução em paralelo e para que esses programas possam compartilhar os recursos da FCTarc13 de forma organizada.  

**Questão 5**:

Problema: Identifique quais são as duas principais funções de qualquer sistema operacional.  

Resposta: Máquina virtual ou máquina estendida (base para a programação), e Gerente de Recursos (possibilita o uso adequado de recursos).  

**Questão 6**: [[Aula 09.16]]

Contexto: A FCT designou a sua equipe para desenvolver um novo sistema operacional “a partir do zero” para certo sistema de computação.

Problema: você deve identificar o "PONTO DE PARTIDA" DO PROJETO, ou seja, POR ONDE COMEÇAR. Interessada em desenvolver um novo sistema operacional para a FCTarc13, a Unesp contratou você para chefiar uma equipe de desenvolvimento, a qual se encarregará dessa tarefa. Como chefe, determine a tarefa inicial do processo de desenvolvimento do sistema operacional da FCTarc13 a ser realizada pela sua equipe.  

Resposta: Pela definição dos principais componentes do SO  

**Questão 7**: [[Aula 09.16]]

Problema: identifique quantos e quais são os principais componentes de qualquer sistema operacional  

Resposta: Quatro Componentes: Escalonador de processos e threads, Gerente de memória, Sistema de arquivo, Software de entrada e saída.  

**Questão 8**: [[Aula 09.18]]

Problema: Mesmo quando um computador está desligado, o seu sistema operacional e os seus programas de usuário permanecem armazenados em um dos seus recursos. Identifique o recurso.  

Resposta: SSD ou HD  

**Questão 9**: [[Aula 09.18]]

Problema: tendo os conceitos de Arquitetura de Computadores em mente, você precisa explicar para os membros da sua equipe qual é a importância do sistema operacional e dos dois programas de usuário serem armazenados no disco rígido ou em outra memória secundária qualquer.  

Resposta:  Quatro Componentes: Escalonador de processos e threads, Gerente de memória, Sistema de arquivo, Software de entrada e saída.

**Questão 10**: [[Aula 10.16]]

Contexto: Assim que o computador é ligado,  

Problema: você precisa descrever resumidamente cada uma das atividades que acontecem no computador da nossa empresa imediatamente após o computador ser ligado; você precisa saber quem é o principal responsável por essas atividades; e você deve deduzir onde o responsável por essas atividades fica armazenado.  

Resposta:  Verifica o setup, faz o POST, descompacta dados, lê dispositivos de armazenamento e carrega o sistema operacional; BIOS; ROM.

**Questão 11**: [[Aula 10.14]] [[Aula 10.16]]

Contexto: Imediatamente antes de encerrar a sua execução, o BIOS da FCTarc13 realiza duas tarefas.  

Problema: precisamos deduzir que tarefas são essas.  

Resposta:  (1) Promove o carregamento do núcleo do sistema operacional a partir do HD ou SSD para a memória RAM e (2) Carrega o endereço da primeira instrução do Escalonador de Processos no IC e no Register of Scheduler.

**Questão 12**: [[Aula 10.21]]

Contexto: Um dos membros da nossa equipe não sabe o que é escalonamento.  

Problema: você deve usar um fato do seu cotidiano para exemplificar o que é escalonamento.  

Resposta:  Turnos de trabalho em uma empresa.

**Questão 13**: [[Aula 11.04]]

Contexto: Você usou um fato do seu cotidiano para exemplificar o que é escalonamento para um dos seus colegas de trabalho.  

Problema: o mesmo colega precisa saber a relação que existe entre  sistema operacional e programas de usuário, e escalonamento.

Resposta:  O sistema operacional e os dois programas de usuário são escalonados para usar o processador

**Questão 14**: [[Aula 11.06]]

Problema: Você deve classificar o seu sistema quanto ao número de programas executados “ao mesmo tempo”.  

Resposta: Multiprogramado

### Factory

O que é um computador? é uma organização de recursos que são submetidos a processos para gerar resultados.

Computadores tem recursos com finalidades específicas.

* Engenharia e Produção - Processador: Unidade de Controle, Unidades Funcionais Diversas
* Vendas - Memória RAM
* Logística - Periféricos
* Almoxarifado - HD ou SSD
* Vigilância - Sensores

O Braço robótico recebe inputs e faz outputs

O sistema operacional é a administração da máquina, gerenciando os recursos e os processos no computador.

O usuário é o cliente, e ele não vê os processos e recursos, para que ele tenha acesso fácil e agradável.

O Processador é gerenciado pelo Gerenciador de Processos

A Memória RAM é gerenciado pela Gerencia de Memória

Os periféricos são gerenciados por Softwares de E/S: Drivers e Rotinas de Serviço

As memórias secundárias, SSD, HD e etc, são gerenciadas pelo Sistema de Arquivos.

As ameaças são gerenciadas pelo sistema de segurança.
