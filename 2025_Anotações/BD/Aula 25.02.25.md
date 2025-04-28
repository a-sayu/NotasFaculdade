Tag: #3_Ano #BD #BDI

---

Modelo Entidade-Relacionamento

Desenvolvido por Chen em 1976.

Utilizaremos o MySQL Workbench, uma aplicação com Interface Gráfica, para se conectar ao MySQL e onde é possível fazer a modelagem do Banco de Dados.

Entidade é um conjunto de objetos do mesmo tipo, exemplo: Pessoa, Aluno, e etc, todos caracterizados por seus atributos. Relacionamentos também podem ter atributos.

Um conjunto de entidades, representa um conjunto de elementos que possuem os mesmos atributos e significados.

O MER não trata entidades individuais, apenas conjuntos de entidades.

Atributos são os valores que representam as propriedades da entidade:
* Monovalorado: possui somente um valor.
* Multivalorado: possui mais de um valor. (Elipse Linha Dupla)
* Composto: atributo com subcampos.
* Derivado: atributos derivados de um outro atributos, ou seja, por exemplo: um atributo calculado. (Elipse Pontilhada)
* Chave: atributo que identifica uma única entidade dentro do conjunto de entidade
* Chave Composta: é um atributo que compõe a chave de um conjunto de entidades. (Termo grifado)

Retângulo: Conjunto de Entidades
Elipse: Atributo

Leitura: Almanaque, Material Complementar

---

## Resumo Aula 2

**Modelo Entidade Relacionamento**:

O modelo não trata de entidades individualmente, apenas o conjunto, que é representado por um retângulo.

**Dados no mundo real** são representados por meio de *conjuntos de entidades*, o *relacionamentos* entre eles e *atributos* que os caracterizam.

**Conjunto de Entidades**:

Conjunto de elementos que tem a mesma estrutura e significado.

**Entidade**: Elemento no conjunto identificado por caracteristicas individuais definidas por atributos.

**Entidade Fraca**: Um conjunto de entidades que não possui identificação própria, pois ela depende de um relacionamento com uma entidade de outro conjunto.

**Atributos**:

Propriedades que descrevem a entidade ou relacionamento entre entidades, são valores que podem ser do tipo:
- Monovalorado; *Valor único.*
- Multivalorado; *Mais de um Valor.*
- Composto; *Possui subcampos.*
- E Derivado. *Deriva de um outro atributo.*

**Chave**: é um atributo que identifica uma entidade dentro de um conjunto de entidades.
- **Chave Composta**: Mais de um atributo compões a chave, ela deve ser o mínimo necessário sem adendos desnecessários.

**Relacionamento**:

Associações entre conjunto de entidades, que podem ser caracterizados por atributos.

**Conjunto de Relacionamentos**: Conjunto de relacionamento de mesmo tipo, representado por um losango, por meio de conceitos como:
- Cardinalidade: *número de entidades que outra entidade pode estar associada em um relacionamento*
- Restrição de Participação: *a dependência de outra entidade por meio de relacionamento*
- Grau de Relacionamento: *número de entidades participantes.*

---

