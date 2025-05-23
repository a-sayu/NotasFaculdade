# Engenharia de Software I

---

Tags: #3_Ano #Es #ESI 

---

Não existe uma **única maneira** de fazer software, como foi falado, não existe uma Panaceia.

> **Panaceia:** *Mecanismos ou práticas que, hipoteticamente, são capazes de solucionar os problemas e/ou dificuldades.* Definição dada por [Dicio](https://www.dicio.com.br/panaceia/)
## Software

**Software** é desenvolvido ou projetado por engenharia, não manufaturado no sentido clássico, não desgasta, mas deteriora com as mudanças do mundo.

Composto por:
1. Instruções: que ao executar produzem a função e o desempenho desejados.
2. Estrutura de Dados: que possibilitam que programas manipulem adequadamente informação.
3. Documentos: que descrevem as operações e o uso dos programas.

O Hardware, que é manufaturado, ele desgasta, sua curva de falhas é como uma bacia.

![[Hardware_Curva_de_Falhas.png]]

Em contrapartida, o software possui uma curva de falhas diferente.

![[Software_Curva_De_Falhas.png]]

A maioria dos softwares são feitos sobre medida, ou seja, com uma utilidade específica única para aquele software.

> *É importante pensar que, se softwares são feitos sobre medida, seu tempo e sua eficiência de trabalho são importantes, então: **Quantas Linhas de Código você produz por hora?**, qual o seu KLOC/h?*

---

### Crise de Software

**Crise se Software**, uma aflição crônica que se refere ao **conjunto de problemas** encontrados no **Desenvolvimento de Software**.
1. Estimativas de Prazo Imprecisas: não há uma coleta de dados sobre o desenvolvimento, nem indicação de produtividade e eficácia de ferramentas, métodos ou padrões.
2. Exigências Vagas: o cliente dá exigências vagas e fica insatisfeito.
3. Qualidade de Software menos adequada: os conceitos de garantia de qualidade começaram a surgir a pouco tempo.
4. Difícil Manutenção: devora o orçamento, e a facilidade não foi enfatizada.

**Causas dos problemas associados à crise de Software:**
1. A própria forma que o software se apresenta, como um sistema lógico e não físico, portanto o sucesso é medido pea qualidade de uma única entidade e não de várias entidades manufaturadas.
2. Falhas das pessoas responsáveis pelo desenvolvimento.
3. Mitos que propagam a desinformação e confusão.

**Mitos do Software** podem ser Administrativos, Clientela e Profissionais.
1. A: Tendo um manual com todos os padrões e procedimentos, isso já não oferece tudo que é necessário saber?
	1. Ele é usado?
	2. Sabe-se que ele existe?
	3. Reflete a prática moderna de desenvolvimento?
	4. Ele é ou está completo?
2. A: As ferramentas de desenvolvimento são de última geração
	1. Muito mais é necessário para desenvolver softwares de alta qualidade.
3. A: Se há atraso, apenas adiciona-se mais programadores
	2. Desenvolvimento de Software não é um processo mecânico, adicionar mais pessoas pode o tornar ainda mais atrasado.
	3. Pode-se adicionar mais pessoas, caso haja um planejamento primeiro.
4. C: Uma declaração geral é o suficiente, detalhes podem ser deixados para depois.
	1. Uma definição ruim --> fracasso no desenvolvimento
	2. É fundamental uma descrição formal e detalhada.
5. C: Requisitos modificam-se continuamente, mas as mudanças podem ser facilmente acomodadas pois software é flexível.
	1. A mesma mudança em estágios tardios do desenvolvimento pode ter magnitudes de demandas e gastos maiores comparados à estágios iniciais.
6. P: Assim que o programa for escrito e estiver em funcionamento, o trabalho está completo.
	1. 50 a 70% de todo esforço gasto são feitos depois que ele foi entregue pela primeira vez.
7. Enquanto eu não tiver ele funcionando, eu não tenho como avaliar a qualidade dele.
	1. O funcionamento é só uma parte da configuração de software, incluindo todos os itens de informação produzidos durante a construção e manutenção.

---

## Engenharia de Software

Em resposta à crise de software, se tem a **Engenharia de Software**, a aplicação de um processo de software sistemático, disciplinado e possível de ser medido.

> **David Lorge Parnas**, pioneiro de engenharia de software, desenvolveu o conceito de ocultação de informações na programação modular, um elemento importante para a programação orientada a objetos. Também conhecido pela defesa da documentação precisa.

Em qualidade de software, aquelas que precisam ser atendidas são atendidas.

O processo de Software abrange três elementos fundamentais:
- Método: o passo a passo do **como**
- Ferramentas: **suporte** para os métodos.
- Procedimentos: o elo entre métodos e ferramentas, com a sequencia, exigências, controle de qualidade e marcos de referência.

**ISO 12207:**
![[ISO12207.png]]
*No Pressman, a estrutura apresentada como processo de software é na verdade a unidade de desenvolvimento de software*

> *A ISO/IEC 12207 é a norma que define processo de Engenharia de Software, atividdes e tarefas que são associados com os processos do ciclo de vida do software desde a sua concepção até a retirada/descontinuação do software.*

**Processo de Software com Qualidade:**

Eficiente, Definido, Gerenciado, Medido, Controlado. Potencial para crescimento e consistência que ele é aplicado em projetos por toda a organização.
- Inteligibilidade
- Visibilidde
- Suportabilidade
- Aceitabilidade
- Confiabilidade
- Robustez
- Manutenibilidade
- Velocidade

**Fases Genéricas dos Modelos de Processos de Engenharia:**
1. Especificação
2. Projeto
3. Implementação
4. Teste
5. Instalação
6. Manutenção

**Fases Genéricas dos Modelos de Processo de Software:**
1. Definição
2. Desenvolvimento
3. Manutenção
4. Atividades de Apoio

### Fase de Definição

> *"O que"*

Ocorrem três tarefas principais: engenharia de sistemas, planejamento do projeto de software e aanálise de requisitos.

Informação processada, Função e Desempenho, Comportamento Esperado, Interface, Restrições Existentes, Critérios de Validação e Tarefas realizadas.

### Fase de Desenvolvimento

> *"Como"*

As três tarefas técnicas que devem ocorrer: projeto de software, geração de código, inspeção e teste de software.

Estrutura dos Dados, Implementação da Função como arq de software, Caracterização de Interfaces, Detalhes, Tradução para uma Linguagem, Efetuação de testes.

### Fase de Manutenção

> *"Mudanças"*

Associada com: Correções, Adaptações e Melhoramentos.

Reaplica-se os passos das fases anteriores, mas faz com o contexto do software já existente.
### Apoio

Essas três fases são complementadas por uma série de atividades de apoio que são plicadas durante toda a engenharia de software:
- Controle e Acompanhamento do Projeto de Software
- Revisões Técnicas Formais
- Garantia de Qualidade de Software
- Gerenciamento de Configuração de Software
- Preparação e Produção de Documentos
- Gerenciamento de Reusabilidade
- Medidas

---

### Modelos de Processo de Desenvolvimento

Cascata: Sequencial Linear
- Faz-se tudo de uma fase para dar entrada em outra.

Prototipação
- Conforme a requisição elaborar um projeto rápido e um protótipo para refiná-lo e obter mais requisitos e detalhamento, para ao ser identificado todos os requisitos, descarta-se o protótipo e constrói-se seguindo os critérios de qualidade.

RAD: Rapid Application Development
- É um modelo sequencial linear que enfatiza o ciclo de desenvolvimento, baseado em componentes. E ao final une-se todos os componentes para formar o produto final.

Evolutivos: Incremental, Espiral, Montagem de Componentes
- Incremental: Cascata + Prototipação.
- Espiral: Um loop de cascata com a ideia da prototipação, sem fases fixas.
- Montagem de Componentes: Classes orientadas a objetos são reutilizáveis em diferentes arquiteturas de sistema.

Quarta Geração
- Especificar o software a uma máquina em um nível próximo a linguagem natural.

(... 🚧 ...)