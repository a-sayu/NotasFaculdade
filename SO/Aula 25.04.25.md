# Sistemas Operacionais II

Tags: #3_Ano #SO #SOII 

---

Hoje é a resolução da questão 47. Terça feira que vêm realizaremos a 39.

---

**Questão 47**: (35) Você está ajudando certa empresa a desenvolver um novo sistema operacional. Problema: você precisa deduzir quantos vetores de interrupção o sistema operacional deve possuir.

**Resposta**: A quantidade necessária de vetores de interrupção para o sistema operacional deve ser a mesma que a quantidade de rotinas de serviço de interrupção, pois no vetor de interrupção estão localizadas os endereços para as rotinas de serviço de interrupção. (O mesmo número de rotinas de tratamento de interrupção.)

Fonte: [Introdução a Sistemas de Computação Digital](https://www.dca.fee.unicamp.br/~leopini/DISCIPLINAS/EA869/2018-1/k1-interrupcao-geral.pdf) e [Interrupções](http://paginapessoal.utfpr.edu.br/kovalhuk/disciplinas-1/el08d-microcontroladores-2/material-das-aulas/gk_2018_01_Aula03-interrupcoes.pdf/at_download/file)

---

**Devolutiva da Questão 37**: A resposta mais correta é que não, é necessário driver. O sistema nem sempre está pronto para trabalhar com recursos principalmente dispositivos periféricos, por isso há a necessidade de instalar programas para dispositivos que não são tão comuns. Drivers são guias/condutores, a ideia é que ele guie o dispositivo periférico mas para o núcleo do sistema operacional, a atividade do driver não é guiar o dispositivo periférico, para Arq. de computadores: SIM, mas como driver é fortemente relacionado à teoria de sistemas operacionais, ele passa a fazer parte do sistema operacional, fazendo parte como componente do SO, assumindo outra responsabilidade.

**Devolutiva da Questão 38**: A resposta é tradutor, o driver traduz aquilo que o programa de usuário, rotina de tratamento de interrupção espera que o recurso faça. Ou seja traduz algo entre o hardware do periférico com a rotina de tratamento de interrupção. Dica: No último jogo (System Call) ele retrata muito bem a parte das questões 35, 36, 37, 38, 47, é possível enxergar como eles trabalham no núcleo do sistema operacinal.