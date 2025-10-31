# 25-ESII-Trabalho

Objetos Humanos: Gerente, Funcionário, Cliente
Objetos: Imóvel, Vistoria, Técnico, Contrato, Seguro, Aluguel, Multa, Agendamento.

- Seguro, Gerente, Funcionário e Cliente $\rightarrow$ Glossário Definição.

## Requisitos

Entrada no Sistema: Login Geral, Cadastro de Funcionários por Gerentes, Cadastro de Clientes por Funcionário, A conta suprema: Primeira Conta.

- Suportar somente entrada de caracteres UTF-8 através do teclado.
- Suportar apenas caracteres não numéricos ou especiais em caracteristicas nomes.
- Suportar no mínimo 60 caracteres em caracteríticas nomes.
- Suportar senhas com pelo menos um caracter alfanumérico minúsculo e maiúsculo, um caracter especial e um caracter numérico.
- Suportar entrada de comandos do mouse.
- Permitir o acesso ao sistema conforme a inserção de um identificador único e a senha correspondente através de uma interface de login.
- Suportar uma interface gráfica para login.
- Permitir o registro no sistema através de uma interface de cadastros.
- Suportar uma interface gráfica para cadastros.
- Criar uma conta de gerente inicial para administração do sistema em geral.
- Reconhecer que o funcionário está conectado apenas na mesma instância do aplicativo ao realizar uma funcionalidade do sistema.

### Login Geral

- Permitir a busca de um funcionário no sistema.
- Ser capaz de reconhecer que o funcionário está conectado em outra instância do aplicativo.
- Ser capaz de verificar a senha do funcionário.

### Cadastro Funcionário

- Reconhecer que um funcionário com cargo gerente está conectado na mesma instância do aplicativo ao realizar um cadastro de funcionário.
- Permitir o cadastro de um funcionário com as seguintes características: nome não vazio, senha de 6 à 8 caracteres gerada aleatoriamente, data de nascimento, cpf, telefone, e-mail, endereço (rua, cep, número da casa, complemento), foto 300x400 pixels do tipo jpeg, gênero (feminino, masculino ou outros), cargo (gerente ou funcionário), salário (numérico).
- Reconhecer se o funcionário sendo cadastrado já existe no sistema.

### Cadastro de Cliente

- Permitir o cadastro de um cliente com as seguintes características: nome não vazio, data de nascimento, cpf ou cnpj, telefone, e-mail, endereço de contato (rua, cep, número da casa, complemento), foto 300x400 pixels do tipo jpeg e gênero (feminino, masculino ou outros).
- Reconhecer se o cliente sendo cadastrado já existe no sistema.

###  Cadastro de Imóvel

- Permitir o cadastro de um Imóvel com as seguintes características: nome não vazio, cliente proprietário não vazio, ocupado (verdadeiro ou falso), tipo de imóvel (casa, apartamento, chácara), laudo técnico não vazio e laudo de vistoria.
- Reconhecer que o funcionário está conectado na mesma instância do aplicativo ao realizar um cadastro de imóvel.
- Reconhecer se o imóvel sendo cadastrado já existe no sistema.

### Criação de Laudo Técnico

- Permitir a criação de um laudo técnico com as seguintes características: nome do responsável não vazio, foto 300x400 pixels do jpeg, endereço (rua, cep, número da casa, complemento), valor do imóvel, área total e área interna.

### Criação de Laudo de Vistoria

- Permitir a criação de um laudo de vistoria com as seguintes características: nome do responsável não vazio e descrição com no máximo 2500 caracteres.

### Criação de Contrato de Aluguel

- Permitir a criação de um contrato de aluguel com as seguintes características: lista de seguros, caução do aluguel, porcentagem de desconto, valor da comissão da imobiliária, cliente locatário, funcionário responsável e imóvel.
- Não permitir a criação caso algum desses esteja vazio.

### Criação de Seguro

- Permitir a criação de um seguro com as seguintes características: valor do seguro, descrição do seguro com no máximo 2500 caracteres, ativação do seguro (verdadeiro ou falso).
- Não permitir a criação caso algum desses esteja vazio.

### Criação de Cobrança de Aluguel

- Permitir a criação de uma cobrança de aluguel com as seguintes características: valor do aluguel, dia do pagamento e pago (verdadeiro ou falso)

### Criação de Cobrança de Multa

-

### Funções de Recursos Humanos

#### Editar Funcionário > Arquivar Funcionário

- Permitir que um funcionário possa editar as seguintes características: senha não idêntica à atual, telefone, e-mail, endereço.
- Permitir que um gerente possa editar todas as características de funcionário de cargo não gerente, tirando senha, data de nascimento e cpf.
- Permitir que um gerente possa arquivar um funcionário em caso de demissão.
- Permitir que o gerente inicial possa editar as caracteristicas de funcionãrios em geral.

#### Editar Cliente > Arquiva Cliente

- Permitir que um funcionário possa editar todas as características de um cliente, tirando a data de nascimento e cpf.
- Permitir que um funcionário possa arquivar um cliente.
- Permitir que o gerente inicial possa editar as características de clientes em geral.

### Funções do Sistema

#### Editar Imóveis > Arquivar Imóvel

- Permitir que um funcionário possa editar todas as características de um imóvel.
- Permitir que um funcionário possa arquivar um imóvel.
- Enviar uma notificação para os clientes relacionados (proprietário e locatário) em caso de arquivamento.

#### Editar Laudo Tecnico > Arquivar Laudo Técnico

- Não permitir que haja alterações em um laudo técnico.
- Permitir que um funcionário possa arquivar um laudo caso haja um outro laudo mais recente criado para o imóvel.
- Enviar uma notificação para os clientes relacionados (proprietário) em caso de arquivamento.

#### Editar Vistoria > Arquivar Vistoria

- Não permitir que haja alterações em um laudo de vistoria.
- Permitir que um funcionário possa arquivar um laudo caso haja um outro laudo mais recente criado para o imóvel.
- Enviar uma notificação para os clientes relacionados (proprietário) em caso de arquivamento.

#### Editar Contrato > Arquivar Contrato

- Permitir que um funcionário possa editar as características de um contrato de aluguel.
- Permitir que um funcionário possa arquivar um contrato de aluguel.
- Enviar uma notificação para os clientes relacionados (locatário e proprietário) em caso de edição ou arquivamento.

#### Editar Seguro > Arquivar Seguro

- Permitir que um funcionário possa editar as características de um seguro.
- Permitir que um funcionário possa arquivar um seguro.
- Enviar uma notificação para os clientes relacionados (locatário e proprietário) em caso de edição ou arquivamento.

### Cobrança

#### Editar Cobrança de Aluguel > Arquiva Cobrança de  Aluguel

- Permitir que um funcionário possa editar as características de uma cobrança de aluguel.
- Permitir que um funcionário possa arquivar a cobrança de um aluguel caso a característica pago for verdadeira.

#### Editar Cobrança de Multa > Arquiva Cobrança de Multa

- 

#### Editar Agendamento > Arquiva Agendamento

- 

### Busca

#### Busca de Imóveis, Seguros, Clientes, Funcionários

- 

### Notificação

#### Cobrança do Aluguel Notificação

- 

#### Cobrança da Multa Notificação

- 

#### Registro de Pagamento

- 


#### Notificação de tudo e todos

- 

### Relatório

#### Relatório Mensal da Imobiliária

- 

### Funções Não Evidentes

#### Cálculo de Aluguel

- 

#### Cálculo de Multa

- 

#### Cálculo do Seguro

- 

#### Cálculo de Despesas

- 

#### Cálculo de Custos

- 

#### Cálculo de Ganhos

- 

#### Cobrança do Aluguel Automática

- 

#### Cobrança da Multa Automática

- 
