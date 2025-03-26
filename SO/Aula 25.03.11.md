# Aula de Sistemas Operacionais

Tag: #3_Ano #SO #SOII

Responder a questão 22 (*Semana Passada*), 23 e 24.

**Questão 22**: A Nossa equipe de trabalho concluiu que divisão de memória para armazenamento de informações parece ser uma prática comum e necessária. Problema: proponha que, além da RAM, o mesmo sistema operacional usado pela nossa empresa divida e controle a divisão de outro tipo de memória para armazenamento de informações.

**Minha Resposta**: O sistema operacional deve gerenciar também a Memória Secundária afim de armazenar as informações necessárias em um sistema de arquivos.

**Resposta Correta**: Está correto a parte de memória secundária. Complementando com o sistema de arquivos, mas é importante mencionar que o núcleo organiza com tanto o gerenciador de memória quanto o sistema de arquivos, sendo importante notar que na memória secundária, é organizado em blocos, que pode ter o menor tamanho de um setor (ArqComp) ou até mesmo mais setores, sendo importante não confundir setor com bloco.

**Questão 23**: Você pôde observar o comportamento do braço robótico enquanto o sistema estava em operação. Problema: com base, exclusivamente, no comportamento do braço robótico, caracterize o algoritmo de escalonamento em relação aos programas de usuários.

**Minha Resposta**: O algoritmo de escalonamento está permitindo uma alternância para os dois programas do braço robótico, permitindo que ele completasse todas as instruções do programa. (Justo)

**Questão 24**: Você pôde observar o comportamento do braço robótico enquanto o sistema estava em operação. Problema: considerando o comportamento do braço robótico, caracterize o algoritmo de escalonamento em relação aos programas de usuário e ao tempo que cada um deles tem para realizar os seus trabalhos.

**Minha Resposta**: O algoritmo de escalonamento como mencionado na 23, é alternado, e o tempo que cada um deles tem para realizar seus trabalhos é o tempo necessário para completar todas as instruções. (Igualitário)
