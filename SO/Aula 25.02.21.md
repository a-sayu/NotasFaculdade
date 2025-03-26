# Aula de Sistemas Operacionais II

Tag:  #3_Ano #SO #SOII

Segunda Aula do Ano de 2025.

## Questão 21

Você já sabe que a memória RAM deve ser particionada (repartida) entre o sistema operacional e os programas de usuário. Problema: a nossa empresa precisa saber em que momento(quando) e como a memória RAM deve ser particionada (repartida) entre o sistema operacional e os programas de usuário.

**Minha Resposta:** O particionamento da memória principal, para que ela se atente ao tamanho dos programas do usuário, ou seja, caso seja de tamanho dinâmico, deve ser feita quando o processo é recebido, ou seja, antecedendo a chegada dele. Caso contrário se o particionamento for fixo, é definido no inicio das atividades do Sistema Operacional, antes de qualquer processo. (Particionamento lógico fixo (no início das atividades do SO) ou variável (durante as atividades do SO) de tamanhos diferentes.)
