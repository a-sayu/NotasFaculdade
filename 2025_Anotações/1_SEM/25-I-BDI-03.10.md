Tag: #3_Ano #BD #BDI

O Atributo chave é o que vai indicar de forma única, cada tupla (cada linha). Apesar do CPF ser único ele não irá possuir a semântica de um RA.

O relacionamento é uma associação de entidades, e deve possuir uma semântica para os dados relacionados. Um conjunto de relacionamentos, é composto por relacionamentos do mesmo tipo.

A notação de relacionamento é o losango. Significando uma associação entre entidades.

Cardinalidade
Cardinalidade 1: 

Cardinalidade Muitos para Muitos: Um funcionário pode participar de quantos projetos? Muitos. Um projeto pode ter quantos funcionários? Muitos. Logo, muitos para muitos.

Cardinalidade Mínima e Máxima, uma notação par (min, max), em que min significa o mínimo de vinculados, e max significa o máximo que pode estar vinculado.

Grau de Relacionamento
Indica quantas entidades podem participar do relacionamento, podendo ser binário, ternário, quaternário e outros, apesar de que é desejável que sejam binários ou ternários para facilitar.

Um relacionamento triplo deve ocorrer ao mesmo tempo, e a cardinalidade se torna complicada, e a quebra de relacionamentos triplos irão perder a semântica.

Uma única entidade pode ter duas ligações, agindo como se fosse um grau ternário.

Auto Relacionamento
É quando uma entidade relaciona com ela mesma.

Entidade Fraca
Uma entidade que não possuem uma identidade própria, ou seja, não é possível identificar ela de forma única, e ela so existe a partir de um relacionamento, e ela tem uma chave parcial. A entidade é identificada por linhas duplas. 

Restrição de Participação
Mostra a dependência de participação de um relacionamento.

Parcial x Total
Uma entidade que só existe se estiver em um relacionamento com outra entidade tem restrição total. No caso em que só uma parte do conjunto estiver relacionado, a entidade tem restrição parcial.

Site de Diagramas de Banco de Dado: https://www.brmodeloweb.com/lang/pt-br/index.html