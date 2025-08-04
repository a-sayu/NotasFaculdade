# Engenharia de Software I

---

Tags: #3_Ano #ES #ESI 

---

## Qualidade de Software

> *Pressman fala muito mal de modelagens, por falta de profundidade, e por isso passamos para o Larman.*

Antes de falarmos a fundo sobre qualidade, o que é para nós alunos? Capacidade de Preencher requisitos.

E como testamos essas qualidade? Tendo parâmetro, depende do propósito, e depois então testar. Sem os dois anteriores, testar é "meio" sem sentido.

Conformidade com requisitos funcionais (faz as ações que são esperadas), com desempenho (nas atividades feitas), e para isso é necessário ter sido explicitamente declarados, cmo padrões de desenvolvimento e documentados, com características implícitas (esperadas).

**Padrões de Desenvolvimento**: Definem um conjunto de critérios que orientam a maneira a qual o software passa pelo trabalho de engenharia, que se não seguido atrapalham o trabalho da engenharia.

**Requisitos Implícitos** como facilidade de uso e desejo de uma boa manutenibilidade, se há falha nisso muito provavelmente falha nos padrões de desenvolvimento e a **qualidade é suspeita**.

Prazo e Orçamento também são uma perspectiva de qualidade.

Funcionalidade importa ao Usuário, defeitos, manutenibilidade e conformidade com requisitos mais os anteriores importam ao Desenvolvedor, prazo, custo, produtividade e os anteriores importam a Organização.

(...)

### Gerenciamento de Qualidade

> *Quem testa é o chato, ele, entretanto, não deve testar a pessoa e sim o artefato recebido para testar*

**Custo de Prevenção**, **Custo de Falhas**, **Custo de Falhas Externas**, **Custo de Avaliação**, há também a quantidade que a imagem comercial foi prejudicada pelos detalhes técnicos.

**Garantia de Qualidade de Software**: um padrão planejado e sistemático de ações que cruzam todas as ações vistas pelo método Larman. Ao cruzar todas as ações do método ele dá a gerencia uma forma de medir a qualidade do produto que sinaliza que o trabalho realmente terminou.

Ae algum problema for identificado, o gerente deve aplicar a correção e por exemplo, treinamento de quem errou.

- Métodos Técnicos para obter especificações de qualidade ou desenvolver um projeto de qualidade.
- Revisão para avaliar qualidade da especificação, projeto, código etc.
- Teste de Software para garantir a detecção de erros seja efetiva, que não necessáriamente seja uma execução de código, pois há testes que não são sempre sobre o código.

---

#### Atividades SQA

> *Existe uma regrinha para os professores formalizados*

Padrões e Procedimentos Formais, Medidas, Manutenção de Registros.

Engenheiros de Software são aqueles que trabalham da construção e o Grupo de SQA está apontando os erros da construção.

- Preparar o Plano de SQA
- Assegurar que as avaliaçãoes estão sendo executadas
- Verificar se padrões estao sendo aplicados
- Possuem um conjunto de documenntos
- Feedback

Dívidas Técnicas.

---

#### Verificação e Validação

> *Teste é uma das atividade de validação*

**Erro**, minimizado pela detecção da presença de erros.

**Verificação**: Contrução correta conforme o que foi combinado nos procedimentos padrões definidos anteriormente.

**Validação**: Resultado correto, se o produto está correto.

**Análise Estática:**
- Revisão, olhar a estrutura.

Isso é uma forma de filtrar a qualidade, e pode ser aplciada em diversos pontos do software. Ele pega a diversidade do grupo, pois funciona para um aprender com o outro, confirmar as partes do produto e realizar o trabalho técnico mais uniforme.

**Análise Dinâmica:**
- Qualquer artefato passível de executar, não necessariamente executando um código.

(...)

**Teste de Software:**

(...)

> *Eu errei, mas o que está lá dentro é um defeito*

Nós procuramos *defeitos* no produto, não erros de pessoas. Em caso de execução não esperado, não é erro, é uma *falha*. E também há o *fault* e o *mistake*.

Mas por enquanto testa-se a presença de defeitos.

**Aspecto Positivo de SQA:**
- Menos defeitos
- Maior confiabilidade
- Custo de vida grobal reduzido: maior demora para o desenvolvimento, mas a entrega vai possuir menos defeitos no futuro.

> *O maior custo está me manutenção, pois é todo o restinho da vida entregue, que pode ser corretiva, adaptativa pois muda-se o software e evolutiva, onde se coloca funcionalidade a mais*

**Aspectos Negativos:**
- Dificilmente instituídos em pequenas empresas, pois o analista único faz de tudo, e SQA se torna um trabalho pesado quando se está sozinho.
- Mudança Cultural

Abre-se uma planilha com a métrica de linhas de código.

**Avisos:**
16/06 - 19/06 sem aula.
23/06, prova adiantada.