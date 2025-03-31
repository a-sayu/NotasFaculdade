# Sistemas Operacionais II

Tag: #3_Ano #SO #SOII

**Questão 26**: Tendo sempre o projeto FCTarc em mente, você deve lembrar que todos os registradores da FCTarc detêm algum tipo de informação, enquanto a FCTarc executa um programa qualquer. Problema: precisamos saber como se chama esse conjunto de informações que a FCTarc tem armazenado em seus registradores a cada instante.

**Resposta**: Contexto, o contexto pode ir além de apenas os conteúdos dos registradores, envolvendo todo o conteúdo dos registradores, mas também dos computadores e informações úteis para manutenção do processo, para que possa ser restaurado após a interrupção.

**Questão 27**:  A sua equipe chegou à conclusão de que ocorre escalonamento entre os processos de usuário responsáveis pelos dois tipos de movimentos distintos efetuados pelo braço robótico. Problema: você precisa explicar como cada processo consegue voltar a ser executado exatamente a partir do ponto em que ele foi interrompido quando o seu quantum expirou.

**Resposta**: Salvamento e Recuperação de Contexto.

**Questão 28**: A nossa equipe já sabe que o contexto de um processo precisa ser salvo e recuperado durante o ciclo de vida de um processo. Problema: precisamos deduzir onde e em que estrutura de dados o armazenamento do contexto dos processos é feito.

**Resposta**: RAM; tabela de processos. É onde o contexto é armazenado, mas dentro da RAM na estrutura tabela de processos.

**Questão 29**: Considere o braço robótico como um recurso compartilhado entre processos de usuários. Problema: proponha uma forma de controlar esse compartilhamento.

**Resposta**:

Processo é o programa e o conjunto de informações necessárias para que o programa seja executado.