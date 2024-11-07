# Prova 2 : POO

Tag: #anotacao_geral #POO2

## Sobre a Prova

* Três Exercícios de resolução prática
* Um exercício teórico
* Um exercício meio teórico e prático.

## Conteúdo

Padrões de Projeto.

---

## Anotações de Revisão para a Prova

### Príncipios de "Bons Projetos"

**Integidade Conceitual:**

Coerência e Padronização de Funcionalidades, Projeto e Implementação.

Por exemplo, se seu projeto utiliza as variaveis assim_assado, devem ser usadas dessa forma até o final do código, para manter a integridade, e não começar a utilizar um AssimAssado no meio do código.

**Ocultamento de Informação:**

Os detalhes internos de uma classe ou módulo devem ser escondidos de outras partes do sistema, apenas expondo o que é necessário.

Por exemplo, um sistema bancário precisa ter acesso ao método de sacar e depositar dinheiro, mas ele não tem acesso ao dinheiro.

**Coesão:**

Uma "unidade" deve ter uma única função/serviço. Unidade sendo classes, funções, métodos, pacotes e etc.

Exemplo, se eu tenho uma classe que serve para representar a pilha, dentro dela somente haverá funcionalidades de pilha, e não de fila!

**Acoplamento:**

Acoplamento é a dependência de uma classe com outras, através de métodos de outras, extendem outras e etc.

Existem dois acoplamentos:

Aceitável e o Ruim

O **Aclopamento Aceitável** depende das duas classes que dependem entre si, em que aquela que depende de outra tem realmente necessidade pelo benefício da outra, a outra "promete" que irá se comportar de certa meneira, e que ela apenas chamará métodos da interface, sem conhecer ou depender de detalhes internos da outra.

O **Acoplamento Ruim** ocorre em duas situações, a primeira quando a classe usada é frequentemente modificada, criando um vínculo frágil e difícil de manter, pois a que depende sempre fica propensas a problemas por conta da classe usada, e segunda quando a classe que depende acessa diretamente a implementação interna da outra, expondo os detalhes e as tornando fortemente dependentes.

### Princípios para Projetos (Incompleto)

**Responsabilidade Única:**

* Segregação de Interfaces
* Prefira Interfaces à Classes
* Aberto/Fechado
* Demeter
* Substituição de Liskov

### Padrões de Projeto: Por que?

**Reuso**, Você pode reaproveitar soluções para problemas recorrentes ao invés de criar uma solução do zero, economizando tempo de desenvolvimento e risco de erros.

**Vocabulário para Comunicação**, quando todos sabem o que significam os nomes dos padrões de projeto, fica mais fácil de entender e alinhar as decisões de design e implementação.

### Padrões de Projeto Criacionais

**Abstract Factory**, é um padrão que permite você ter famílias de objetos relacionados sem ter que especificar suas classes concretas ao usá-las.

Um jeito de entender é que o cliente apenas deseja criar **um objeto de uma família**, ele não quer ter que especificar o tipo que ele está criando durante todo o código, pois se mudar o cliente terá que mudar todo o código! É muito mais fácil se tivermos que **mudar uma linha do que todas**, certo?

**Quando Usar?** Situações que você pode avaliar de usar Abstract Factory:

* Trabalhar com famílias de objetos relacionados, ou seja, não depender das classes cruas/concretas daqueles objetos, de forma que você destaque que: é possível **trabalhar sem se comprometer** com a implementação específica desses objetos, permitindo expandir no futuro.
* **Garantir a não inconsistencia** dos objetos criados, pois todos os objetos irão estar em uma mesma variante padronizada, garantindo que objetos criados por uma fábrica pertençam a mesma família.
* Extrair métodos de uma **classe sobrecarregada**, ou seja classes que não seguem o princípio de responsabilidade única e possuem métodos de criação que tiram o foco de sua "responsabilidade principal"

* Singleton

### Padrões de Projeto Estruturais

* Proxy
* Adapter
* Facade
* Decorator

### Padrões de Projeto Comportamentais

* Strategy
* Observer
* Template Method
* Visitor
