# Aula de Programação Orientada a Objetos II

Tag: #POO2

Realizamos alguns Exercícios sobre Propriedades de Projeto.

TODO: Reler os exercicios da página 51 em diante e realizá-los.

## Princípios de Projeto

### 1- Responsabilidade Única

Cada classe de negócio deve ter uma única responsabilidade lógica ou regra de negócio, ou interface, permitindo ser usada por mais de uma outra classe.

Interface x Negócio = Frontend x Backend

### 2- Segregação de Interfaces

Interfaces devem ser pequenas, coesas e específicas para cada tipo de cliente.

### 3- Inversão de Dependências

O não uso de inversão de dependências é demonstrado por uma necessidade de uma especifidade que não torna possível interagir com qualquer tipo.

Com a Inversão de dependências você se preocupa apenas com o genérico. "Prefira Interfaces à Classes".

### 4- Prefira Composição a Herança

Herdar deve ser feito para especialização.

1. "é-um" -> herda atributos e métodos de motor
2. "possui" -> possui um atributo

No primeiro caso, se tem um "extends", mas no segundo apenas se instancia a outra classe, tornando desnecessário o uso de uma herança.
