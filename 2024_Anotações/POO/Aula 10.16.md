# Aula de POO

Tag: #2_Ano #POO2

## Padrões de Projeto

Utilidades:

* Reusar o projeto, não precisar reinventar algo.
* Mesmo vocabulário para comunicação

Padrões:

* Criacionais: Factory, Singleton
* Estruturais: Proxy, Adapter, Facade, Decorator
* Comportamentais: Strategy, Observer, Template Method

Padrões de projeto auxiliam em design for change (Projetar com a intenção de otimizar mudanças), em caso de que o código dificilmente mude, usar padrões é um "overengineering"

### Fábrica

Padrão de Projeto que possui uma interface para criar objetos em uma classe super, mas permitindo que subclasses também alterem o tipo dos objetos que serão criados.

* Centralizar a criaçao de certos objetos.

### Singleton

;

* Unificar em uma única instância, portanto um Singleton

### Proxy

;

* Objeto intermediário entre clientes e objetos base, de forma que o cliente não fale diretamente com o objeto, tendo que passar por um proxy primeiro.

### Adaptador

;

* Uma classe adaptadora que cria um mediador que traduz um conteúdo para outro

### Fachada

;

* Criar uma interface mais simples, realizando todas as "chamadas" que são "encheção de saco"

### Exercícios

1,2- Singleton pode causar problemas de design, pois componentes do programa ficam sabendo demais sobre o outro, em um ambiente de processamento em paralelo deve possuir um tratamento especial para não se criar diversos objetos singleton.

### Decorador

É um design estrutural que permite atribuir novas funcionalidades à objetos colocando esses objetos dentro de objetos 'pacotes'

### Estratégia
