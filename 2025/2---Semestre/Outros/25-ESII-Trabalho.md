# 25-ESII-Trabalho

Objetos Humanos: Gerente, Funcionário, Cliente
Objetos: Imóvel, Vistoria, Técnico, Contrato, Seguro, Aluguel, Multa, Agendamento.

- Seguro, Gerente, Funcionário e Cliente $\rightarrow$ Glossário Definição.

## Requisitos

Entrada no Sistema: Login Geral, Cadastro de Funcionários por Gerentes, Cadastro de Clientes por Funcionário, A conta suprema: Primeira Conta.

- Suportar somente entrada de caracteres UTF-8 através do teclado.
- Suportar apenas caracteres não numéricos ou especiais em caracteristica nome.
- Suportar senhas com pelo menos um caracter alfanumérico minúsculo e maiúsculo, um caracter especial e um caracter numérico.
- Suportar entrada de comandos do mouse.
- Permitir o acesso ao sistema conforme a inserção de um identificador único e a senha correspondente através de uma interface de login.
- Suportar uma interface gráfica para login.
- Permitir o registro no sistema através de uma interface de cadastros.
- Suportar uma interface gráfica para cadastros.
- Criar uma conta de gerente inicial para administração do sistema em geral.

### Login Geral

- Permitir a busca de um funcionário no sistema.
- Ser capaz de reconhecer que o funcionário está conectado em outra instância do aplicativo.
- Ser capaz de verificar a senha do funcionário.

### Cadastro Funcionário

- Reconhecer que um funcionário com cargo gerente está conectado na mesma instância do aplicativo ao realizar um cadastro de funcionário.
- Permitir o cadastro de um funcionário com as seguintes características: nome não vazio, senha de 6 à 8 caracteres gerada aleatoriamente, data de nascimento, cpf, telefone, e-mail, endereço (rua, cep, número da casa, complemento), foto 300x400 pixels do tipo jpeg, gênero (feminino, masculino ou outros), cargo (gerente ou funcionário), salário (numérico).
- Reconhecer se o funcionário sendo cadastrado já existe no sistema.

### Cadastro de Cliente

- Reconhecer que um funcionário está conectado na mesma instância do aplicativo ao realizar um cadastro de cliente.
- Permitir o cadastro de um cliente com as seguintes características: nome não vazio, data de nascimento, cpf ou cnpj, telefone, e-mail, endereço de contato (rua, cep, número da casa, complemento), foto 300x400 pixels do tipo jpeg e gênero (feminino, masculino ou outros).
- Reconhecer se o cliente sendo cadastrado já existe no sistema.

### Funções de Recursos Humanos

>  Registro Funcionário > Editar Funcionário > Arquivar Funcionário

- Permitir que um funcionário possa editar as seguintes características: senha não idêntica à atual, telefone, e-mail, endereço.
- Permitir que um gerente possa editar todas as características de funcionário de cargo não gerente, tirando senha e cpf.
- Permitir que um gerente possa arquivar um funcionário em caso de demissão.


Registro de Cliente > Editar Cliente > Arquiva Cliente
**`TODO`**

Funções do Sistema:
Registro de Imóveis > Editar Imóveis > Arquiva Imóvel
**`TODO`**

- Criar Imóvel (reconhecer se nome não vazio, caracter alfanumérico, gerar , preencher dados (algum dado)

Registro de Tecnico > Editar Tecnico > Arquiva Técnico
**`TODO`**

Registro de Vistoria > Editar Vistoria > Arquiva Vistoria
**`TODO`**

Registro de Contrato > Editar Contrato > Arquiva Contrato
**`TODO`**

Registro de Seguro > Editar Seguro > Arquiva Seguro
**`TODO`**

Registro de Aluguel > Editar Aluguel > Arquiva Aluguel
**`TODO`**

Registro de Multa > Editar Multa > Arquiva Multa
**`TODO`**

Registro de Agendamento > Editar Agendamento > Arquiva Agendamento


Busca de Imóveis, Seguros, Clientes, Funcionários


Cobrança do Aluguel Notificação


Cobrança da Multa Notificação


Registro de Pagamento


Notificação de tudo e todos


Relatório Mensal da Imobiliária


Funções Não Evidentes:
Calculo de Aluguel


Calculo de Multa


Calculo do Seguro


Calculo de Despesas


Calculo de Custos


Calculo de Ganhos


Cobrança do Aluguel Automatica


Cobrança da Multa Automatica

