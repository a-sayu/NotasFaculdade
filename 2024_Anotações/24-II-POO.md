# Prova 2 : POO

Tag: #anotacao_geral #2_Ano #POO2

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

* Responsabilidade Única
* Segregação de Interfaces
* Prefira Interfaces à Classes
* Aberto/Fechado
* Demeter
* Substituição de Liskov

[Link para uma resposta do chatgpt](https://chatgpt.com/share/672ce053-af50-800b-bfb8-f8b8cc38d87e)

### Padrões de Projeto: Por que?

**Reuso**, Você pode reaproveitar soluções para problemas recorrentes ao invés de criar uma solução do zero, economizando tempo de desenvolvimento e risco de erros.

**Vocabulário para Comunicação**, quando todos sabem o que significam os nomes dos padrões de projeto, fica mais fácil de entender e alinhar as decisões de design e implementação.

### Padrões de Projeto Criacionais

#### Abstract Factory

**Abstract Factory**, é um padrão que permite você ter famílias de objetos relacionados sem ter que especificar suas classes concretas ao usá-las.

Um jeito de entender é que o cliente apenas deseja criar **um objeto de uma família**, ele não quer ter que especificar o tipo que ele está criando durante todo o código, pois se mudar o cliente terá que mudar todo o código! É muito mais fácil se tivermos que **mudar uma linha do que todas**, certo?

**Quando Usar?** Situações que você pode avaliar de usar Abstract Factory:

* Trabalhar com famílias de objetos relacionados, ou seja, não depender das classes cruas/concretas daqueles objetos, de forma que você destaque que: é possível **trabalhar sem se comprometer** com a implementação específica desses objetos, permitindo expandir no futuro.
* **Garantir a não inconsistencia** dos objetos criados, pois todos os objetos irão estar em uma mesma variante padronizada, garantindo que objetos criados por uma fábrica pertençam a mesma família.
* Extrair métodos de uma **classe sobrecarregada**, ou seja classes que não seguem o princípio de responsabilidade única e possuem métodos de criação que tiram o foco de sua "responsabilidade principal"

##### Método de Fábrica Estático

**Demonstrado em Slide**: Foi utilizado o método de fábrica estático, em que se cria um método estático (public static) que reduz a necessidade de instanciar um objeto só para chamar um método de criação, é interessante caso métodos não vão ser alterados no futuro por subclasses.

#### Singleton

**Singleton**, é um padrão que permite garantir uma instância única para uma classe, provendo um acesso global para essa instância.

Todas as implementações do Singleton tem duas coisas em comum:

* Constrtor padrão Privado (Não permiter um new)
* Método estático de criacão que chama o construtor privado para o criar e salva em um campo estático de forma que todas as chamadas seguintes retornem um objeto já existente.

**Quando Usar?** Situações que o padrão Singleton pode ser aplicado:

* Quando se precisa de uma única instância compartilhada com todos os clientes.
* Um controle mais estrito sobre variáveis globais, sem o risco de duplicar a instância.

### Padrões de Projeto Estruturais

#### Proxy

**Proxy**, é um padrão que permite fornecer um substituto/espaço reservado à um objeto, controlando o acesso ao objeto original.

**Mas por que controlar acesso?**, supondo que você tenha um objeto que consome muitos recursos do sistema, mas não precisa dele sempre, você pode adiar a criação dele, mas essa lógica resultaria em código duplicado (o cliente checa se precisa criar).

O proxy resolve o problema acima criando um intermediário que simula a classe original, ele atrasa a sua criação até o momento que for realmente necessário.

Basicamente, ele chama na primeira execução e nas próximas, enquanto não houver modificação no objeto, chamará o objeto criado guardado.

#### Adapter

**Adapter**, é um padrão que permite objetos incompatíveis colaborarem entre si.

Usando esse padrão, ao invés de modificar o codigo (que talvez você não tenha acesso, talvez possa quebrar algum outro código que depende dele), você cria um objeto especial que converte a interface de um objeto para que outro possa entendê-lo.

A melhor analogia para o Adapter é o adaptador de tomada.

**Por que usar o Adapter?** Situações que o padrão Adapter pode ser aplicado:

* Quando quer usar uma classe existente, mas a sua interface não é compatível.
* Quando você quiser reutilizar diversas subclasses existentes que não possuam uma funcionalidade comum que não pode ser adicionada a superclasse (se assemelha muito a um decorador)

#### Facade

**Facade**, é um padrão que fornece uma interface simplificada para um biblioteca, framework ou conjunto complexo de classes, o não uso de um fachada ao usar um conjunto complexto tornaria seu código muito acoplado aos detalhes de classes de terceiros, tornando difícil de entender e compreender.

Com a fachada, ela fornece uma interface simples para um subsistema com muitas partes, fornecendo ao cliente apenas as funcionalidades que ele se importa.

O cliente não precisa saber o que você está instanciando, o formato de um arquivo que vai ser sempre o mesmo e etc!

**Quando Usar?** Situações que o padrão Fachada podem ser aplicados:

* Quando é necessário uma interface simplificada para um subsistema complexo, mostrando apenas o essencial.
* Quando quer estruturar um subsistema em camadas, reduzindo o acoplamento entre subisistemas, mantendo a comunicação organizada e independente (similar ao mediador)

#### Decorator

**Decorator**, é um padrão que permite que você acople novos comportamentos para objetos colocando-os em "pacotes" que contem esses comportamentos.

**Quando Usar:**

* Precisa adicionar comportamentos adicionais, por exemplo em execução, sem quebrar o código que usa esses objetos
* Quando o padrão é complicado ou impossível de estender com herança

### Padrões de Projeto Comportamentais

#### Strategy

* Strategy

#### Observer

* Observer

#### Template Method

* Template Method

#### Visitor

* Visitor
