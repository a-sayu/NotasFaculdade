# Sistemas Operacionais II

Devolutiva da questão 31. Aula de hoje será a solução do problema 32, que é diretamente relacionado ao problema 31. Até da para juntar as duas questões, mas pode complicar o trabalho pela maior demanda de criatividade. Haverá uma devolutiva complementar sobre as chamadas do sistema ou na próxima aula, ou na semana que vêm.

Os processos de usuario não controlam diretamente o recurso, pois se fizessem isso, eles monopolizariam os recursos, então uma maneira de evitar o monopólio, é fazer com que a alocação de recursos e projetos seja controlado pelo núcleo do sistema operacional, e quando um processo precisa de um determinado recurso ele precisa solicitar ao núcleo no sistema operacional, e essa solicitação, formal, é chamada de chamada do sistema.

Processos sempre irão fazer isso sempre que estiverem em execução.

---

**Questão 31**: Você já sabe muito bem que, para o sistema apresentado pela nossa empresa, o braço robótico é um recurso compartilhado entre processos de usuários. Problema: proponha uma forma de controlar esse compartilhamento, sem que os processos de usuários sejam responsáveis por ele. Em outras palavras, explique como seria esse controle.

**Resposta**: Chamada de Sistema, é a resposta mais correta.

**Questão 32**: Observe mais uma vez o comportamento do braço robótico enquanto o sistema está em operação. Problema: deduza em que momentos (quando) ocorrem chamadas de sistema, enquanto o sistema apresentado pela nossa empresa está em operação

**Resposta**: Quando no quantum de um processo que precisa de algum recurso compartilhado em sua execução, ele pausa a si mesmo com uma chamada do sistema, para que o sistema agora tome controle e forneça o recurso ao processo para continuar sua execução. (Para envios de comandos ao robô e finalização dos processos.)

