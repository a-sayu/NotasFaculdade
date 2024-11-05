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

O Aclopamento Aceitável depende das duas classes que dependem entre si, em que aquela que depende de outra tem realmente necessidade pelo benefício da outra, a outra "promete" que irá se comportar de certa meneira, e que ela apenas chamará métodos da interface, sem conhecer ou depender de detalhes internos da outra.

### Princípios para Projetos

* Responsabilidade Única
* Segregação de Interfaces
* Prefira Interfaces à Classes
* Aberto/Fechado
* Demeter
* Substituição de Liskov

### Padrões de Projeto Criacionais

* Abstract Factorey
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
