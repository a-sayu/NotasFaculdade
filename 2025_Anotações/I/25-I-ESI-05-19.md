# Engenharia de Software I

---

Tags: #3_Ano #ES #ESI 

---

## Devolutiva da motivação da Prova

A prova é interessante para identificar como os conceitos estão interligados, as operações para escolher eram check_in e check_out, era também válido qualquer outra, mas era um de cada para aprofundamento. Era possível colocar a quantidade que quisesse, mas o importante era mostrar que se sabia o que estava sendo feito.

Para o modelo conceitual, se houvesse os conceitos básicos estava valendo, era de se ter todos os conceitos interessantes mostrados na descrição, sendo que no mínimo era necessário ter check in e check out.

Se fosse uma questão de cada uma, era feito mais questões, mas não era para destrinchar o que era cada coisa e sim uma compreensão de como as coisas estavam interligadas e como essas coisas auxiliam uma a outra.

A intenção da exatidão das páginas para essa prova era saber narrar toda a ideia, para não se ter uma falta de noção de espaço de escrita.

A correção será feito possívelmente no outro próximo final de semana.

## Padrões de Projeto

### Breve Revisao de Diagrama de Classes

Pontilhado no Diagrama de Classes indica que a visibilidade não é como uma de constante, ocorrendo de forma temporária, portanto, não é visível sempre.

Enquanto ele cria-se um item ele enxerga algo durante um curto tempo, o caminho pontilhado não é mantido.

### Padrões

É recomendado fortemente a leitura do livro. O que é padrão? *Algo normatizado, repetido, acordo. Algo que pode ou deve ser seguido*, este é a primeira ideia, mas o padrão do sentido de: definir uma forma que não necessáriamente está em norma, em que não se está normatizado, mas há um jeito padronizado de se fazer, portanto seguir diretamente à solução, não se fazendo por ser regra, mas para se resolver um problema.

É uma convenção que resolve problemas por experiência, o passo-a-passo da solução é que fornece um padrão.

O padrão surgiu na área da Arquitetura e Urbanismo, em que se deixava o caminho ser formulado pelas pessoas para após construir a calçada.

Padrões de Arquitetura, Padrões de Projeto, Padrões de Código, Padrões de Padrões... Elas são usadas em vários contextos.

> ***Padrão** é uma descrição nomeada de um problemas e uma solução*

### GRASP

General Responsability Assignment Software Patterns, essa associação de responsabilidade que é definida no padrão GRASP.

Alguns padrões principais GRASP são:

Especialista, Criador, Coesão Alta, Acoplamento Fraco e Controlador.

O Controlador é quem controla as camadas do sistema.

### Controlador

Quem é responsável por tratar eventos do sistema? A responsabilidade deve ser atribuida à classe que represente todo o sistema, dispositivo ou subsistema, chamado de controlador de fachada.

> *O **Melhor** é criar outro*

Mas porquê? Se criar dois controladores de fachada, separar ou unir é um *depende*, a vantagem da união é a facilidade e controle de tudo, o deixando inchado. Mas separado há também uma questão de quem é o controlador de tudo? Portanto é será então melhor ter um controlador dos controladores?

Normalmente se faz o segundo do controlador de pequenos controlador, para distribuição da operação, não por ser melhor ou por padrão.

> *Esse negócio de melhor, não é sempre que é o melhor*

Geralmente se cria um controlador para um caso de uso, do jeito feito na análise de casos de uso que se verifica a mehor forma para a criação de um controlador de fachada.

Como deve ser a posição de controladores? Por clique/interação ou por toda a produção do caso de uso.

#### Discussão

Controladores de Fachada deve ser um objeto que sugira uma cobertura sobre outras camadas e que seja o ponto principal, pode ser uma abstração física ou lógica. No exemplo muda-se a interface/camada de interface, mas não a de domínio, pois não muda-se as regras de domínio, apenas da interface.

Deve se ter um controlador diferente por caso de uso, se há divisão de casos de uso, por que se dividiu? A justificativa da decisão da divisão é a justificativa de um controlador. Se há um controlador muito inchado, talvez seja necessário separar.

Não se aparece no modelo conceitual por não ser um objeto do domínio, apenas algo que controla os objetos do domínio.

#### Controladores Inchados

Controles com falta de foco, tratando de muitas responsabilidades, alguns sinais são:
- Uma única classe tratando **todos** os enventos, sendo comum em controladores de fachada.
- O Próprio controlador executa as tarefas necessárias, sendo que sua função é delegar para outras classes.
- Um controlador tem muitos atributos, ele deveria ser como uma marionete, que mexe por cordinhas pois a marionete não guarda informações, ela não deve duplicar atributos que estão abaixo.

A **cura de controladores inchados** é acrescentar controladores e delegar responsabilidades.

> *Objetos de Interface (Janelas) não são controladores, elas não devem ter a responsabilidade de tratar eventos.

À um tempo atrás se era ensinado fazer justamente colocar um grid, e usando esse grid colocar a tabela no grid, e ao se ver a interface, há uma tabela que diretamente atualiza o banco de dados. Mas nisso quebra-se padrões e acabar com o banco de dados.

> *Não se deve expor nada na interface sobre o que ocorre no domínio, pois o que deve ir para cima o que de fato deve estar acima.*

#### Benefícios

Aumento de possibilidade de reutilização e também o conhecimento do estado do caso de uso, pecebendo então se já se foi feita a entrega, não sendo necessário passar por algum caso de uso já pronto, facilitando as coisas sobre um outro caso de uso.

### Comentário do Professor

Em uma startup, se há uma ideia, demontra-se que é boa e consegue-se o investimento de alguém. Qual o esforço para algo de fato ir para a venda como produto final? Melhora-se a estrutura do projeto, arquitetura de software. Reescrita da ideia escalada para ser vendida. 
### Especialista

Ao longo dos slides se percebe já o padrão do especialista que apresenta um problema de responsabilidade de um objeto, com a solução de atribuição sobre ele mesmo, pois ele é o especialista sobre a informação dele mesmo, diminuindo o acoplamento entre as classes.

É o padrão mais utilizado e óbvio, e que tem uma analogia na vida real.

É um benefício pois mantém o encapsulamento já que o comportamento fica distribuído entre as classes que tem a informação necessária. Porém é contra indicação quando se aumenta o acoplamento e reduz a coesão.

### Criador

(...)

Como objetivo, ele deve definir como criador o objeto que precise ser conectado ao objeto criado, algumas vezes o candidato ao criador é quem tem os dados iniciais. E ele favorece o acoplamento fraco.

### Acoplamento

Ele mede o quanto um objeto conectado tem conhecimento de ou depende de outros objetos.

**Fraco:** Não depende de muitos outros -> Se for zero não dá certo.
**Forte**: Depende de muitos outros -> Se está muito dependente não é bom.

Um acoplamento alto dá efeitos colaterais em outras classes, que se for o oposto há menos impacto em outras classes, minimizando o impacto. Um acoplamento alto também dificulta a ompreensão do objetivo de cada classe além de dificultar o reuso da classe.

Um acomplamento fraco favorece a baixa dependencia e aumenta reutilização.

Como se mede o acoplamento? Pelo número de classes que ele interage.

Quais são as formas de acoplamento?

#### Discussão

Com um acoplamento fraco, há classes mais independentes, considerando em conjunto com outros padrões, e o extremo não é desejável.

Deve ser tentado manter o acoplamento fraco em pontos de evolução ou de alta instabilidade, ou seja, pontos que há certeza de mudança ou alteração, em que o acoplamento não deve subir de forma alguma, ou seja, que a manutenção vai ocorrer e deve-se estar preparado.

Com benefícios falta de impacto por mudanças,fáceis de compreensão e convenientes para reutilização.
### Coesão

Mede o quanto as responsabilidades de um elemento são fortemente focalizzadas e relacionadas.

A coesão alta mantem a complexidade sobre controle. A coesão e o acoplamento andam de mãos dadas.

Assim como Acoplamento Fraco deve ser considerado no projeto de objetos. Classes com coesão alta tem um número de métodos relativamente pequenos.

**Aula finalizada**.