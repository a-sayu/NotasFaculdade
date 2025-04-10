# Engenharia de Software I

Tag: #3_Ano #ES #ESI 

---

**Responsabilidade**
A classe tem a obrigação de fazer uma coisa ou saber de algo, responsável por fazer e por saber os objetos que ela tem.

Responsabilidade pode ser deduzida por modelo conceitual (atributos, associações)

Devemos pensar também na granularidade da responsabilidade, ou seja, a responsabilidade de cada objeto, não é porque foi delegado à um que não se pode distribuir a responsabilidade para os menores.

**Brincadeira 1**: O objeto vai e escreve no quadro
Caminho, Base, Tabela, Quem Grava

O problema, é que todos os objetos precisam ter acesso a isso, mas se todos os objetos precisam fazer isso, cria-se vários trabalhos e métodos distribuidos para muitos objetos.

**Brincadeira 2**: Com um mediador no meio escrevendo no quadro
A responsabildade se torna do objeto mediador

O problema, é o gargalo, criando um grande aclopamento e uma enorme responsabilidade de diversos objetos à um só. Melhora de um lado, mas talvez não de outro, pelo sobrecarregamento, sendo necessário balancear, algo que a arquitetura que resolve.

As duas soluções funcionam, mas há vantagens e desvantagens para os dois tipos.

Visibilidade é gambiarra, é a capacidade de um objeto ver ou fazer referência a outro, o que não deve ser usado.
- Atributo: Existe por apenas um tempo, necessária para uma aplicação significativa, sendo necessária o registro, sendo a maneira mais comum, se devendo as associações. Para quem ele quiser mandar algo, ele deve ter um atributo apontando para o objeto que ele quer se comunicar. Em que a associação vira um atributo que tem que enxergar outra classe. (Ouvir o audio para entender o que ele quis dizer com temporario e refrmular a formatação)
- Parâmetro: Neste momento que está criando o item ele vê a especificação, mas ao sair do método ele perde o parâmetro, ele não sabe mais a especificação do produto, pois quando chamou veio a referência como parâmetro, e o item guardou e mantem, mas o superior perde. (Passo a passo pois é engenharia)
- Localmente Declarada: 
- Global: Não deve ser usado.

<<Associação, Parâmetro, Local>> é pleonasmo na notação em UML, mas é indicado usar. Pois ao denotar a mensagem já indicamos como funciona.

**Diagramas de Colaboração**
A criação é o momento que o projetista deve pensar acerca da arquitetura em totalidade, sendo a hora de pensar, a fase mais criativa da fase de projeto.

É a forma de fazer não para resolver, mas abrir e vizualizar em toda a funcionalidade e evitar criação de novos problemas, baseando-se em bom senso, racíocinio e conta.

**Casos de Uso**: Origem ao diagrama de sequencia.
**Diagrama de Sequencia**: inicia o diagrama de colaboração.
**Diagrama de Colaboração**: Abrem a caixa preta do sistema, e as interações e trocas de mensagens.

E essas interações por mensagens os nomes inspirados pelos termos do modelo conceitual.

- A primeira mensagem é o primeiro evento do diagrama de sequência.
- Se muita complexidade : Separa-se em diagramas menores.
- Não necessariamente deve se chegar na persistência. Não é necessário modelar até lá, mas considerar que decisão deve ser tomada.

(...)

Portanto podemos ter um tratador de eventos, em que internamente vai assumir que todos os eventos serão assumidos por ele, em que (...)

(...)

Batata x Televisão, regras de negócio diferentes, especificações diferentes.

(...)

Diagrama de Casos de Uso justifica a implementação de serialização e Json.
- Deixar a inicialização por último, garantindo que todas as informações necessárias estarão nas classes
	- Criar o objeto incial do domínio
	- Pode ou não assumir o controle, normalmente não
	- Um diagrama de colaboração com primeira mensagem
	- Opionalmente um outro que executa o objeto inicial

Em um sistema real, as especificações estarão em um meio de armazenamento permanente. Inicialização é o último caso de uso a ser feito.

---