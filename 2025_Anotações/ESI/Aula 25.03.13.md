# Engenharia de Software I

---

Tag: #3_Ano #ES #ESI

---

## Branch

Sempre a partir de uma linha base se cria uma ramificação, um galho. Nesses galhos, ela não sofre alterações de outros galhos, sendo necessário juntar com a base original.

Algo a estar atento é a sobreposição de arquivos que estrague algo já feito ou corrigido, sendo importante ser feito por script, programando como fazer a junção, tendo um sistema de controle de versão (VCS), que alerta erros desse tipo.

A junção de galhos é feita através de um *pull request*, que precisa ser aceita antes da mescla seja efetuada, significa que alguém deve olhar, para retornar um feedback sobre aceitar ou não, portanto é o primeiro mecanismo de homologação técnica, não necessariamente a aceitação para o cliente. O Check In, não é o *pull request*, mas engloba o *pull request*.

***

## Engenharia de Requisitos

Saber exatamente o que o sistema irá fazer, basicamente como se fosse o título de um trabalho. Processo de Engenharia de Requisitos é o primeiro passo, em que qualquer que seja o modelo de processo de software.

**Requisitos são uma necessidade que o sistema/produto deve cumprir.** E a engenharia é justamente ter uma abordagem sistemática para compreender o que o sistema deve fazer, ou seja, entender, escrever e passar adiante, o primeiro problema da engenharia de requisito é a comunicação.

Portanto para poder satisfazer é importante se expressar bem. Especificação é diferente de Requisitos.

Elicitar: Deixar Claro. Modelar e Analisar. Este processo precisa de diferentes pontos de vista.

Universo de Informação é o contexto de desenvolvimento de um sistema. Neste local, ou seja, o contexto de um termo, ação e função. Sendo importante descrever esse universo, portanto a partir desse universo, se deixa claro, gerar o documento de requisitos, analisar e tomando decisões de análise, modelar o sistema.

Elicitar é deixar claro, é algo em evolutivo, pois deixa-se claro de pouco em pouco, como uma lamparina numa noite escura, não é um processo rápido. EM que se capta os requisitos, através de:
* Identificação de Fontes de Informação
* Coleta de Fatos
* Comunicação: o método de receber os fatos, as informações.

Análise, identificar as partes do documento de requisitos que devem ser analisados, para depois implementar, priorizando os requisitos mais importantes, portanto a partir do universo de informação para então modelar conforme o que é completo e correto.

Modelos são um jeito de desenhar os requisitos, descrevendo estaticamente e dinamicamente o que o sistema deve fazer, possuindo varias perspectiva do desenho. Importante Representar (Tipos, Relações, Operações), Organizar (Nível de Abstração, Refinamento, Consistência) e Armazenar.

Documento é resultado da elicitação, contendo requisitos funcionais e de qualidade. Não se pode se escrever de forma abstrata, pois é uma forma de comunicação, importante entregar aquilo que está escrito.

Requisitos Funcionais:
* O que o sistema deve fazer. Identificados e Listados em agrupamentos lógicos.
* Funções devem ter um ou mais requisitos. (2 a 3 linhas no máximo)
* Podem ser evidentes, ocultos ou de enfeite (nao afeta significantemente).

Requisitos de Qualidade:
* Qualidades, características ou dimensões que não são funcionais do sistema, normalmente transversal de uso para todos os outros requisitos.
* ISO 9126, seis características de qualidade de software em alto nível, e também que não é necessário ter todos.

1. **"O sistema deve..."** + frase curta.
2. ?
3. Requisitos devem ter identificadores únicos.
4. Requisitos devem estar divididos em funcionais e nao funcionais
5. Evitar decisões de projeto. -- Não deve conter detalhes de implementação.
6. Explicação de termos não deve estar nos requisitos. -- E deve ser consistente no uso desses termos.