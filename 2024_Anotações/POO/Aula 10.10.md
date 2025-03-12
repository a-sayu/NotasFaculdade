# Aula de Programação Orientada a Objetos II

Tag: #POO2

Continuação dos princípios de projeto.

TODO: Estudar atentamente, como perdeu quase que todo o restante dos princípios. pág 92.

## Princícios de Projeto

### 5- Princípio de Demeter

Evitar longas cadeias de chamadas de métodos, promovendo o encapsulamento e reduzindo o acoplamento entre classes.

Um objeto deve se comunicar apenas com os objetos mais próximos e não se intrometer em detalhes internos de outros objetos.

Entretanto, casos isolados podem existir e justificarem o uso de cadeias de chamadas de métodos.

### 6- Princípio Aberto/Fechado

Uma classe deve estar fechadas para modificações, mas aberta para extensões.

É necessário fazer com que a classe possa estender o sistema sem modificar o código existente, permitindo criar códigos que adicionam novos comportamentos sem alterar o código já existente.

### 7- Princípio de Substituição de Liskov

São boas práticas referentes ao uso de herança, especificamente para redefinição de métodos em subclasses.

Substituições de A por B podem ocorrer desde que B tenha os mesmos serviços que A.

Ou seja, se há algo em A, B deve ter também!
