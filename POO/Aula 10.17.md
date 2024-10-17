# Aula de POO2

Todo padrão de projeto cria acoplamentos, evitar de criar por criar e sim por utilidade e ganho;

**Fabric**, se tem uma classe que fabrica, se altero algo, altero apenas a fabrica e não a classe que está sendo usada.

**Singleton**, se não tiver cria-se, se tiver, já a utiliza.

**Proxy**, ele representa a classe, controlando o acesso ao objeto original.

**Adaptador**, se assemelha à tomada, ele adapta o genérico para o específico.

**Fachada**, você cria uma nova classe que apenas passando o parâmetro, não precisa passar por diversas funções para poder usar o objeto desejado, facilitando o uso do cõdigo.

**Decorador**, ele atribui novas funcionalidades colocando pacotes sobre ele.

**Strategy**, permite você criar uma familia de algoritmos em uma classe separada, permitindo "mudar" o código trocando apenas o objeto utilizado.

**Observador**, se cria um mecanismo para notificar multiplos objetos sobre qualquer evento que acontecem com o objeto que estão obbservando.

**Template Method**, implementa-se um esqueleto de um algoritmo em uma classe abstrata, deixando pendentes alguns passos permitindo customização sem mudar a estrutura.

**Visitor**, adiciona uma operação genérica em uma familia de classes, sem mexer no código deles, permitindo que se separe algoritmos dos objetos que eles operam.

## Quando não vale a pena usar

* Uso precipitado e exagerado de padrões de projeto, se a mudança é zero, não precisamos de padrões de projeto.
* Trade-off, para permitir prontidão para mudanças, irá criar complexidade, pois demandam criação de classes extras.

## Trabalho

Uso de mais de dois padrões de projeto.
