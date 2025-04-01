# Sistemas Operacionais II

Tag: #3_Ano #SO #SOII 

Hoje haverá a resolução da questão 30, mas irei fazer a resolução da questão 29 também, caso não haja a devolutiva da questão 29 ainda hoje.

---

**Questão 29**: Considere o braço robótico como um recurso compartilhado entre processos de usuários. Problema: proponha uma forma de controlar esse compartilhamento.

**Resposta**: Respondi que para controlar o compartilhamento pode ser feito uma sinalização para indicar se o braço robótico está disponível para ser usado por outro processo. (Uso do mecanismo de sincronização: mutex.)

Mutex é o mais correto, pois é um dos mecanismo de sincronização, sendo o suficiente para esse problema.

**Questão 30**: Mais uma vez, considere o braço robótico como um recurso compartilhado entre processos de usuários. Problema: tente reconhecer se há algum problema em deixar processos de usuários responsáveis pelo controle do compartilhamento do braço robótico.

**Resposta**: Pois um dos processos pode monopolizar o uso do braço robótico (Monopólio)

Monopólio.

Próxima aula haverá uma devolutiva mais apropriada, e problema 31.