# Engenharia de Software I

Tag: #3_Ano #ES #ESI 

Temos agora que evoluir para o construir, transição do Scrum para o método Larman.

Aperfeiçoar o plano é a última atividade de planejar e elaborar, fazendo um link com Construir em Refinar.

---

Refinar Modelo Conceitual
Anteriormente listamos os substantivos, para vermos o que é substantivo e o que é atributo.

Tipo do Atributo: É opcional nessa etapa, e se for colocar é algo alto-nível, não há necessidade de um vinculo com a linguagem. No Astah, se você escolher Java irá colocar todos os tipos de Java disponíveis.

Os atributos vêm do documento de requisitos. De onde veio os casos de uso, de onde veio o modelo conceitual, Documento de Requisitos e Casos de Usos, é de onde surgiram os atributos e Conceitos.

Um Documento de Requisitos é não completo e não inteiro e portanto evolui, afinal está em um ciclo.

Generalização e Especificação, ainda está sendo desenhando o problema, mas ao refinar o problema me aproximo da solução.

Generalização é buscar um conceito que possui subtipos.

Regra do Um é Um. Exemplo: Pagamento e Pagamento com Cartão, um Subtipo é um Supertipo.

Regra dos 100%, a definição de um supertipo deve ser aplicada ao subtipo, ou seja, há 100% de conformidade com os elementos de um supertipo.

Quando definir um subtipo, depende da relevância para o problema, não é necessário detalhar sempre. Se houver método, associação, comportamentos diferentes, é necessário separar.

Posso Especializar indo para os subtipos, e posso generalizar indo para os supertipos.

> Métodos aparecerão na fase de projeto.

Classes Associativas, em que seus atributos estão relacionados a uma associação e não a um dos conceitos envolvidos a um dos conceitos. 

> t: preciso ouvir os áudios... Eu não entendi bem esse negócio de classe associativa pq acabei perdendo uma parte entre especialização e classe associativa.

Um atributo está relação não à uma classe. Imaginemos um casamento, a data está relacionado ao casamento, e não as duas pessoas, pois armazenar-se-ia duplicado.

Agregação por Composição
Losango preenchido. É uma dependência em tempo de vida, por exemplo se eu cortar a mão, e perco os dedos.

Agregação Compartilhada
Losango não preenchido. É uma dependência sem relação de tempo de vida, por exemplo, se apagarmos um software, as bibliotecas utilizadas por esse software continuariam existindo.

---

Definir Diagramas de Sequência

Na fase de análise, há uma interação com o sistema, uma caixa preta na atual fase, faz-se uma sequencia de operações na linha de tempo do sistema. Esses diagramas saem do caso de uso expandido. Não há if's e else's.

Como dar nome para os Eventos

Por verbos, pois denota ações.

- Para cada Caso de Uso se faz um diagrama de sequência, colocando-se dentro dele. A Elipse de cada Caso de Uso tem que se ter no mínimo um diagrama de sequencia

---

Definir Contrato de Operação

Não se faz para qualquer sistema, se faz para quando há um comportamento esperado, mas sem redundância, sem inconsistências, ou seja, para casos de consequência drástica, operações relevâncias com consequências graves.

É uma segurança para quem faz o sistema, sendo rigoroso e trabalhoso.

---

Definir Diagramas de Estado

Dado um estado, aconteceu um evento, mudou de estado. Pode ser por UML ou por Redes de Petri.

> Dar uma olhada no que é Redes de Petri.

---

Conclusão

- Casos de Uso: Processos do Domínio
- Modelo Conceitual: Conceitos/Objetos
- Diagrama de Sequência do Sistema: ...
- Contratos de Operação: ...

---

Lembrando

Foi feita a análise, e então se começa a projetar para construir, em começo se faz a análise das coisas mais importantes na etapa atual.

Erro Clássico: Fazer tudo no primeiro Ciclo de Desenvolvimento, isso é cascata, não ágil.

Portanto, na P1 é até a fase de análise.

- Larman é melhor para a Classe Associativa.