# Engenharia de Software I

Tags: #3_Ano #ES #ESI 

---

(...)

Eu preciso estar com o diagrama completo para fazer o diagrama de classe? Não. Estará apenas aquilo que está pronto para ser implementado e entregar. Apenas as que vão ser entregues que precisam estar documentadas bonitinhas.

Deve ser feito a medida que avança no desenvolvimento.

**Criação do Diagrama de Classes:**

Estático:
1. Identificar classes a partir dos diagramas de colaboração
2. Acrescentar os atributos identificados no modelo Conceitual
3. Acrescentar métodos provenientes dos diagramas de colaboração
4. Acrescentar tipos de atributos parâmetros e retornos de métodos

Comportamento:
1. Acrescentar associações e navegabilidade (Visibilidade por Atributo)
2. Implementar relacionamentos de dependência (Visibilidade não implementada por Atributo)

1 --- Identificando as Classes. Diagrama de Colaboração

De onde vêm as classes, já possuia no modelo conceitual. Importante notar que um vetor de uma classe não precisa ser uma classe.

2 --- Identificar Atributos. Modelo Conceitual

Pegar os atributos e trazê-los do modelo, e também do diagrama de colaboração.

3 --- Acrescentar os Métodos.

Ou seja, pegar as ligações dos diagramas de colaboração, todos os métodos serão colocados com os parâmetros, se houver retorno e etc. Para todas as classes.

Atenção: Dependendo da linguagem de programação, é recomendado usar sintaxe básica UML O método criar() é dependente da linguagem. Não incluir gets & sets, não incluir métodos correspondentes à mensagens enviadas as classes coleções.

4 --- Tipos Parametros e Retornos

4.1 --- Tipo, o ideal é sim escrever o tipo.

Mas dependendo pode-se deixar. Quanto mais detalhes, melhor é o código gerado, pois reduz o gap semântico na geração. Mas se for somente para desenvolvedores, o escesso de informação pode atrapalhar.

5 --- Associações e Navegabilidade

São indicadas pelo diagrama de colaboração, ela indica o sentido de navegação na associação, e não o sentido de leitura, no modelo conceitual a notação é por seta contínua, mas no caso aqui, nem sempre. Quando à indícios, comunicação entre classes, criação entre classes, mantido a conexão entre classes.

(...)

Não é necessário demonstrar que uma classe associada está no diagrama, pois a representação dele está na associação e se criaria um Pleonasmo.

(...)

6 --- Relacionamentos de Dependência

A seta agora é tracejada, pois uma classe enxerga algo temporariamente, pois no momento que há ponteiro ele enxerga, mas quando acaba o uso ele não enxerga mais, pois o ponteiro não existe mais.

**Padrões de Projeto**

Serão tratados na aula que vêm, retratados no livro do Larman.