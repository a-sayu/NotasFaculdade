# Documentação e Produtividade com Markdown (Obsidian e GitHub)

Abigail Sayury Nakashima abigail-sayury-nakashima | a-sayu

QR Code do Questionário Inicial

## Obsidian

> "Ué, não é um minicurso de Markdown? Por que começar pelo Obsidian?"

O Markdown pode ser o foco do minicurso, mas apesar de podermos trabalhar com o Markdown diretamente, o foco é desde o começo já apresentar a linguagem em uso. E para isso, usaremos o Obsidian como nossa ferramenta de documentação.

### Porque usar Obsidian e não outras ferramentas?

O Obsidian é um software de base de conhecimento pessoal e registro de anotações criado em 2020, ele opera com base em Markdown. Mesmo não sendo open source, além de ser gratuito, caso você não queira mais utiliza-lo ele permite manter seus arquivos localmente e continuar editando eles.

O Obsidian também possui muitas funções, plugins e customizações, e um design bonito e funcional.

Além de permitir criar um Zettelkasten, que é uma caixa de notas interconectadas, que consiste em pequenas anotações guardadas em fichas que podem ser conectadas umas as outras a partir de um assunto principal.

No método do Zettelkasten você teria quatro tipos de notas, notas rápidas, notas de leitura, notas permanentes e notas de referência.

Notas Rápidas são notas de conteúdo curto, usadas para capturar ideias no momento.

Notas de Leitura são notas feitas durante ou depois de uma leitura ou aula de conteúdo.

Notas Permanentes são notas feitas consolidando o conhecimento, relacionando com outras notas.

Notas de Referência são notas que organizam ou explicam o sistema, podendo ter índices, legendas, explicações e convenções usadas.

O Obsidian também permite mostrar um gráfico de conexões entre as notas, e você pode ver tudo que está conectado por links dentro dele.

### Exemplo de Anotações

Exemplo de uma das minhas anotações feita em aula:

![](file://C:%5CUsers%5CCliente%5CAppData%5CRoaming%5Cmarktext%5Cimages%5C2025-09-30-11-51-55-image.png?msec=1759243915650)

Se vocês notarem, algumas coisas são diferentes no meu Obsidian. Git, Excalidraw, Templater, WakaTime e Similar Notes.

### Exercício: Criação do Vault

A princípio, vocês vão ter um obsidian cru, então a gente vai passo a passo construir um Vault ou Cofre e preencher ele com coisas que possam permitir funcionalidades extras que a longo prazo são muito úteis.

Plugins Recomendados: Git, Excalidraw e Templater.

Atividade: Configurar o obsidian, e pegar notas reais de aula, notas sobre o minicurso ou um texto fornecido para testar as funcionalidades do Obsidian integrado com o Git.

_A gente vai fazer o seguinte, caso alguém tenha anotações feitas em aula pode ser, caso alguém não tenha, pode ser as anotações sobre o minicurso ou pode ser até mesmo um texto aleatório, caso alguém não tenha eu vou passar um textinho que eu fiz, que pode estar, inclusive cheio de erros, mas não comentem kk._

## Markdown

Agora vem a parte que talvez vocês tenham lido e pensado no porquê e tiveram curiosidade em participar.

### Por que um Minicurso de Markdown?

Quando se pensa em fazer anotações, podemos pensar em cadernos, Docs, Word, Notion ou mesmo LaTeX.

Mas vocês já pensaram em usar Markdown?

Markdown é uma linguagem de marcação simples, criada em 2004, que converte texto em HTML, e pode ser usado para READMEs e arquivos RTF.

E ele é simples. Legível mesmo sem renderização, funciona em qualquer editor e o foco está no conteúdo e não na formatação.

### Pontos pela qual Markdown é superior à ferramentas comuns de anotação.

Eu gosto muito do markdown comparada as outras ferramentas, claro muitas delas é só skill issue ou frescura, mas esse minicurso não tem a intenção de te fazer abandonar os outros métodos de anotação, mas apenas apresentar uma ferramenta que tem seus usos, e que eu gosto muito.

Cadernos, escrever é lento, não dá para se comparar o tempo digitando com o tempo que passamos escrevendo de forma legível. A não ser que você seja lento digitando, no entanto é uma habilidade que pode ser treinada, e que é muito prática no dia a dia.

Microsoft Word, é útil, mas o docx não pode ser facilmente editado em qualquer editor de texto, e você não consegue abrir em editores simples, como bloco de notas.

Google Docs, é uma ferramenta que eu gosto também, e para o escritor médio, está ótimo, no entanto eu particurlarmente não gosto de depender inteiramente do online, além de que sofre do mesmo problema do Word.

Notion, é uma ferramenta muito útil, mas depende também do online, além do fato de ter um limite que restringe muito o armazenamento.

TXT, é offline, pode abrir em qualquer lugar, é simples, mas é feio.

LaTeX, para anotações em aula parece overkill, além de ter de modo geral uma curva de aprendizado muito maior. Além do fato de apesar ser legível como arquivo de texto para compilar em um documento pdf por exemplo, há todo um trabalho de instalação extra.

E pronto, vamos usar Markdown. Ele é simples, acessível e simples de ser entendido.

E voi la, tá ai o motivo de usar Markdown, haha, nem um pouco talvez forçado e que não precisava de tudo isso... O Markdown é simples, além de poder ser lido como um texto simples e ser facilmente entendido.

### Demonstrar Exemplos de Markdown.

![](file://C:%5CUsers%5CCliente%5CAppData%5CRoaming%5Cmarktext%5Cimages%5C2025-09-30-12-38-01-image.png?msec=1759246681506)

Ali vocês podem ver um pouco de uso de HTML, o que é permitido dentro do Markdown, ou seja, quer enxer de frufru, você pode! No entanto a sintaxe básica é essa, texto puro que renderiza dessa forma:

![](file://C:%5CUsers%5CCliente%5CAppData%5CRoaming%5Cmarktext%5Cimages%5C2025-09-30-12-39-21-image.png?msec=1759246761368)

E como pode-se perceber, tirando o HTML, a parte normal do texto, onde só há Markdown não tem grande diferença comparado a renderização, pois é fácil compreender a mudança.

### Estrutura Básica do Markdown

Vamos fazer de forma didática.

Digamos que eu queira fazer o titulo de um texto, mostrar qual o tópico! Eu poderia deixar esse algo sublinhado, e isso funciona no Obsidian, mas é padrão? Não necessariamente, existem várias implementações do Markdown, e eu vou apresentar algumas formas de fazer coisas no Obsidian e de forma geral.

Então como faço um título? Vamos pensar, vocês já fizeram estrelinha para indicar que algo é importante? Algo como:

⭐Título

Se sim, ao invés de estrela, temos uma #, e quanto mais #, menor o nível de importância dos títulos, na escrita acaba sendo muito fácil escrever, pois na maior parte do tempo você não vai tratar do tópico mega específico dessa forma, e sim com outras formas, como identação do texto, negrito, ou perceber que talvez os tópicos sendo tratados poderiam ser notas mais separadas entre si.

Então vamos agora de forma mais dinâmica e rápida.

Para listas, é só seguir o padrão usado ao escrever:

* ou -, fácil né?

*Itálico* é uma enfase suave, nisso você põe um pouco de brilho com * em volta.

**Negrito** é a enfase pesada, nisso põe mais brilho com ** em volta.

Lista de Tarefas é só pensar em criar as caixinhas que você vai assinalar:

- [x] Tarefa

E se completar

- [ ] Tarefa

Adiciona um X, fácil de ver?

Para fazer linhas de separação entre tópicos, você pode fazer três - ou três *

A tabela é a coisinha mais complicada e chata, onde você tem que pensar nas linhas, como por exemplo esse cronograma:

| Hor | Seg | Ter | Qua | Qui | Sex |

| --- | --- | --- | --- | --- | --- |

| 14h | ES1 | BD1 | PDI | ES1 | --- |

E acaba que nesses casos, apesar de ser fácil escrever e visualizar, é uma das percas de eficiência, e nisso eu deixo o Obsidian fazer, se tornando mais fácil do que colocar passo a passo.

|Hor|Seg|Ter|Qua|Qui|Sex|
|---|---|---|---|---|---|
|14h|ES1|BD1|PDI|ES1|---|

E por final, os menos convecionais de visualizar:

Link e o Link para imagem (Que exibe ela):

[\texto](link)

e ![texto alternativo](imagem.png)

> Citações, com >, nisso ele cria basicamente uma caixinha com o texto dentro.

Código: existem duas formas, o que é o inline só com ` em volta da frase, e o com ```, que cria um bloco de código onde você pode escrever diretamente e ele fica como se fosse txt, a não ser que você adicione a linguagem, e então o obsidian mostra o texto colorido como se fosse um código dentro linguagem.

O markdown, na maioria das vezes consegue integrar com KaTeX, e ai quem sabe LaTeX pode se divertir, meu uso mesmo é só para matemática, como por exemplo essa integral: $$\int^2_0{\frac{\ln{x^2}}{x}}$$, mas as vezes se torna mais prático desenhar do que escrever diretamente.

A parte de HTML, eu fico devendo, porque eu realmente não sei muito de HTML para ajudar. Alguns exemplos podem ser, centralização:

(Exemplo)

### Exercício: Estruturar o arquivo no Obsidian

Lembram daquele arquivo no Obsidian que a gente colocou no cofre? Pois bem, a gente vai estruturar ele em Markdown.

## Documentação

### Por que se preocupar com a documentação

A primeira coisa vista em um projeto no GitHub é o README, uma documentação mal feita atrapalha o entendimento do funcionamento, o objetivo, o que está completo e o que torna seu projeto único.

Uma boa documentação deixa claro as funções e features do seu código, a intenção por trás, indica a etapa do desenvolvimento, atrai contribuições, facilita manutenções, servindo como manual e também o que torna seu projeto único.

### Exemplos de Boas e Más Documentações de Repositório.

![](file://C:%5CUsers%5CCliente%5CAppData%5CRoaming%5Cmarktext%5Cimages%5C2025-09-30-13-21-06-image.png?msec=1759249266565)

![](file://C:%5CUsers%5CCliente%5CAppData%5CRoaming%5Cmarktext%5Cimages%5C2025-09-30-13-22-03-image.png?msec=1759249324014)

### Ensinar tópicos importantes a se considerar quando documentando seu repositório

Normalmente você deve incluir na sua readme:

- O que faz
    
- Porquê ele é útil
    
- Como usar
    
- Como contribuir
    
- Quem mantem/contribui
    

### Exercício de Estruturar um README de um repositório do GitHub.

Escolha um projeto seu, que não possui um readme, e a gente vai estruturar ele.

## Conclusão

### Exercício Opcional de pegar uma anotação de aula real e estruturar em um Vault com todo o conhecimento adquirido.

Lembra do Obsidian? Pois então, vamos colocar esse vault no github!

Ficar a disposição para tirar dúvidas.

### Questionário de opinião sobre a aplicação de Markdown, GitHub e Git e Obsidian e se o Minicurso foi útil e pontos a melhorar (Dar exemplos de pontos a melhorar)

QR Code do Questionário Final