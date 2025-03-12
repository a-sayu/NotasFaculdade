# Aula de Sistemas Operacionais II

Tag: #SO  #SOII

Primeira Aula do Ano de 2025, continuação da disciplina de Sistemas Operacionais.

## Questão 20

A sua equipe concluiu que a memória RAM deve ser particionada (repartida) entre o sistema operacional e os programas de usuário. Problema: você precisa reconhecer se há algum problema relacionado a tamanho e, em seguida, você precisa propor uma maneira de particionar a RAM entre o sistema operacional e os programas de usuário levando esse problema em consideração.

**Minha Resposta:** Quando se utiliza partições de tamanhos fixos, ocorrem dois tipos de problemas em relação ao tamanho dessas partições, se a partição é maior que o programa que vai ser executado, o restante do espaço nessa partição é perdido, e se as partições disponíveis são menores que um programa a ser carregado e não são contínuas para se somarem, em que a memória perdida fora da área ocupada por um processo. Uma forma de particionar que é através de partições variáveis, em que o tamanho das partições é ajustado dinamicamente às necessidades exatas dos processos. (Programas possuem tamanhos diferentes; particionamento em tamanhos diferentes)

**Resposta Correta:** 
