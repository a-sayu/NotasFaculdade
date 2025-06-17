# Sistemas Operacionais II

---

Tags: #3_Ano #SO #SOII 

---

Questão 45: Problema: nossa empresa espera que você seja capaz de explicar a diferença entre um programa ser executado no modo núcleo e outro ser executado no modo usuário.

**Devolutiva da Questão 45**: Tudo que é do núcleo do sistema operacional roda em modo protegido  modo nucleo modo supervisor, portanto somente programas especificos do nucleo do programa operacional podem acessar determinado superconjunto de programas da maquina reservados para atividades especiais, chamadas críticas, e por isso so o nucleo do sistema operacional tem acesso a esse subconjunto de instruções, todas as demais instruções da maquina que não são consideradas criticas podem ser acessadas pelos demais programas.

A última questão 46.

Questão 46: Problema: com base na observação do slide intitulado “Unidade de Gerência de Memória”, deduza o que a MMU faz.

**Devolutiva da Questão 46**: O que estudaremos mesmo é a configuração interna de uma MMU (Unidade de gerenciamento de memória), ou seja, nosso foco principal para esse problema está na MMU. A MMU, apesar de ser estudada em SO, ela poderia ter sido estudada na disciplina arquitetura de computadores, pois tudo que esta sendo visto, costuma-se ser implementado em hardware, pois é uma unidade funcional que auxilia o computador em relação a gerencia de memória.

No semestre passado, foi comparado a memoria principal com a memória secundária, e que foi comparada a um armário. A memória é como se fosse uma caixa vazia disponivel para armazenar informações, mas as informações não podem ser jogadas de qualquer forma, o ideal é que elas sejam organizadas na memória.

Particionamento: O processo deve caber inteiramente em uma única partição

Segmentação: É uma outra maneira de se organizar, em que os processos podem estar espalhados pela memória ou seja seguimentados.

Vantagens da Segmentação: Impedir a ocorrencia de fragmentação da memória, a grande vantagem é reduzir o desperdício de memória RAM.

Em que no caso do particionamento fixo ocorria fragmentação interna, que era ter uma area maior do que a necessária para o processo, e o particionamento variavel ocorria a fragmentação externa, era que sobravam buracos muito pequenos entre as áreas da memória, dificultando a formação de novos particionamentos para outros processos.

Segmentos podem ter tamanhos diferentes e são melhor adptados a partes especificas do processo, com um desperdício desprezível.

Desvantagem da segmentação: Complexidade. Suas partes espalhadas com tamanhos diferentes torna a gerencia mais complexa do que anteriormente, com o gerente passando a ser maior e mais complexo e dificil de ser projetado e implementado e consequentemente mais caro. Todos os equipamentos que estão sendo lidados no dia a dia trabalham com segmentação.

Normalmente quando um computador trabalha com segmentação, ela não vem sozinha, ela normalmente vem acompanhada da memória virtual e da paginação que auxiliam na compreensão da MMU.

É bem comum na computação termos processos, ou até mesmo, o próprio programa dentro do processo, tendo um tamanho maior que a area de memória física disponibilizada para ele, programa no caso entede-se como processo, e memória física como memória RAM.

Ou seja, processos que o tamanho superam o tamanho total da memória RAM ou a área disponibilizada para o processo.

Nós sabemos que um processo para ser processado, ele até pode ser armaenado na memoria secundaria, mas ele deve ser processado no processador, e a diferença de velocidade entre os dois é muito grande, principalmente se for disco rígido. Então entre a memória secundária e os registradores internos do processdor, se tem um subsistema de memórias para que a diferneça e velocidade não seja sentida pelo usuário da máquina (RAM, CACHE, NIVEIS de CACHE).

Mas a memoria ram continua tendo um tamanho epqueno que a memoria virutla, entao ele não pode ser armazenado interiramento na memoria RAM, e por isso ele tem que ser armazenado em pequenas areas, portanto se tem o conceito de paginação.

Mas enfatizamos o modelo de paginação, o processo dentro da memória virtual pode ser comparado a um livro e todo livro possui páginas, e esses pequenos retangulos são chamaados de paginas, que possuem informações.

As informações estaram distribuidas em diferentes paginas que são pequnas comparadas ao tamanho total do processo. E na memoria fisica tem subdivisões com tamanhos coincidentes com os tamanhos das paginas, a memoria ram esta subdividida em molduras para as páginas

O que não estiver em uso ficara na memoria virtual, so indo o conjunto de informações que estiver sendo buscado para ser processado no processador, e esse subconjunto de paginas recebe um nome nomeado de cnojunto de trabalho, que são as paginas escolhidas pela gerencia de memoria para ocupar as areas disponíveis na memória RAM.

A questão mais delicada é que, os numeros representam os endereços na memória virtual que interessa apenas para o próprio processo, que somente ele conhece, o que esxiste d verdade é o espaco de endereçamento fisico reais presentes na memoria RAM, quando uma pagina esta na memoria virtual as suas informações são referenciadas com base no espaço de endereçamento na memoria virtual, mas ele muda pois passa a ser no espaço de endereçamento físico.

Que então a gerencia deve procurá-las, passando a mão para o MMU.

O MMU tem um registrador em cima, um registrador em baixo e uma pequena memória que pode até ser um conjunto de registradores que pode ser mais rapido, cada um com uma finalidade especifica, e este registrador aqui guardara o endereco virtual da informação que esta sendo buscada na memoria principal, o de baixo ira guardar o endereço real da informação que esta sendo buscada na memoria e a tabela é uma simples tabela de conversão, do endereço virtual para o endereço real.

MMU: hardware que auxilia a gerencia de memoria em converter endereços virtuais em reais.

Mais significativos do virtual = indexar a tabela, e o endereço correspondente a esses quatro bits mas que está na tabela, amrazena o endereço da moldura da pagina que contem a informação requisitada para compor o endereço fisico, os 4 bits mais significativos que representam o endereço virtual, são substituidos elos tres bits mais significativos do registrador que representam a molsdura da pagina real, o restante e simplesmente copiado, e desta forma os endereços fisicos sao mapeados nos virtuais.

É como se houvesse uma associação direta cm base da pagina direta dessa pagina para a moldura ali.


