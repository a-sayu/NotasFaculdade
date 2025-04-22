# Fundamentos de Processamento de Imagens

Tag: #3_Ano #PDI 

---
## Olho Humano

Almir está explicando sobre o funcionamento do olho e qual parte que importa, no caso, a retina, pois a luz através do olho e projeta-se na retina, em um ponto chamado Fovia (importante), onde se possui detalhes.

O que são bastonetes e cones na retina?

É importante saber como o olho funciona para atender suas necessidades e se aproveitar das limitações. 

* Ponto Cego do olho
* Percepção do Olho
* Ilusão de Ótica

**Daltonismo**, e como ela afeta a percepção das cores em programação e imagens.

**Influência de uma vizinhança na análise visual**, em que por exemplo um tom próximo de algo mais escuro parece mais claro, e esse mesmo tom perto de um mais claro parece mais escuro.

É necessário reconhecer as **limitações** do olho humano, como por exemplo a distinção de tons vizinhos de cinza.

## Modelo de Formação da Imagem usando Iluminação

Função 2D de f(x, y), que é positiva e finita, ou seja maior que 0 e menor que o infinito. Essa função pode ser obtida por uma i(x, y)r(x, y), em que i é a intensidade de luz, e r a refletância, ou seja a quantidade de luz refletida pelos objetos.

Em convenção de coordenadas em uma imagem digital, se tem, começando em zero até n-1 tanto no eixo x, quanto no y, para os ambientes de programação se inicia no 1 até n.

As imagens podem ser representadas por uma matriz com M linhas e N colunas, onde cada elemento da matriz é chamada de pixel.

## Sensores

Câmeras são feitas de sensores de energia, onde sai um sinal elétrico e uma saída proporcional à entrada. Esses censores são os CCD, charge-coupled device, em que cada CCD captura a integral da energia incidente em sua superfície.

**Linear**: Usado em Scanners. De forma que diminui o custo de comprar inúmeros sensores, comparados à um Matricial.

Outro tipo de escaneamento é com um cilindro, e um sensor que o analisa em volta dele.

Sensores não são digitais, eles são analógicos, são sinais que possui virgula basicamente, criando uma necessidade de conversão à sinais digitais.

**Questões fundamentais:**

Amostragem: Discretização do Espaço

Quantização: Discretização da Intensidade (Níveis)

Em um sinal analógico, o sinal vai de -1 a 1, de forma que há infinitos valores entre eles. Um computador digital não trabalha com números infinitos, e por isso é necessário discretizá-lo, convertendo-o em um sinal digital.

Por isso uma imagem fica pixelada, pois ocorresse a amostragem (de quanto em quanto farei a coleta), ou seja o tamanho do pixel. E a quantização diz o que é alto/baixo, claro/escuro.

Amostragem de uma suposta câmera de baixa amostragem: 200x200 pixeis.
Quantização seria quantas cores que a máquina captura.

24 bits é o mesmo que 2^24 chamado pelo Almir de true color.

****

A regra é encontrar qual a frequência mais alta do sinal analógico, para de obter a taxa de amostragem, que seria então no mínimo duas vezes o valor da frequência máxima.

dpi = pontos por polegada.

Saturação é quando ao aproximar altos valores de brilho, apenas fica branco, parecendo algo não natural de cor. Ruído é uma granulação na textura.

Quanto mais se captura, melhor a qualidade, se usa-se poucos níveis, se apresenta poucas cores.

Como é feito o calculo de tamanho de armazenamento, pois então, largura x altura x o que cada caixinha também está armazenando, se for colorida, se tem x 3. NxMxk, k = qtd. de tons. É fácil imaginar como se fosse um cubo deformado pela "profundidade" de k em cada posição (nxm).

### Interpolação de Imagem

Muito utilizada em tarefas de ampliação e encolhimento, rotação e correções geométricas, usando de dados conhecidos para estimar valores em locais desconhecidos, uma forma de visualizar essa ampliação é criar uma grade imaginária 750 x 750 com o mesmo espaçamento da imagem original e então encolher essa grade até se enquadrar na imagem original.

O método do vizinho mais próximo duplica pixeis, deixando ela cheia de pixeis apenas, maiores. Deixando uma distorção em arestas retas.

Outra melhor abordagem é a **bilinear** que é basicamente a duplicação só que com uma média entre os dois valores, interpolando tanto na linha quanto na coluna, usando 4 vizinhos mais próximos. Pensa em uma cruz, que analisa o que deveria ter no centro dessa cruz com base nas quatro pontas.

O valor é atribuído da seguinte equação:

$v(x, y) = (v(x-1, y) + v(x+1, y) + v(x, y-1) +v(x, y+1))/4$

Um jeito de calcular é fazer também, linha sim, linha não, e depois calcular as colunas, nas linhas faltantes.

Interpolação Bicúbica, ela permite que as curvas sejam suaves. Ela pega dois pontos, e ao interpolar, você olha dois para um lado e dois para o outro, encontrando a interceptação das duas linhas do lado. 

### Relação entre Pixeis

Um pixel tem quatro vizinhos, vizinhança-4 é a vizinhança dos quatro vizinhos padrões (N4), e a vizinhança diagonal é os quatro vizinhos na diagonal desse pixel (Nd), e o conjunto desses dois é N8

**Conectividade**, dois pixeis estão conectados se eles estiverem na vizinhança e seus níveis de cinza satisfazem uma similaridade.

Conectividade 4, p e q são conectados no conjunto dos 4.
Conectividade 8, p e q são conectados no conjunto dos 8.
Conectividade m, em que p e q são conectados ou pelo conjunto dos 4, ou pelo conjunto dos D, mas ainda não se conhecem, evitando um caminho "duplo" da conectividade 8.

**Medidas de Distância**, deve ser maior ou igual a 0, a distancia deve ser igual das duas direções e a soma de duas outras distancias deve ser igual ou maior que a distancia de um dos pontos de uma distancia para o outro ponto da outra distancia que não há em comum. (p, q) + (q, z) >= (p, z)

**CityBlock x Xadrez x Euclidiana**

Operações Aritméticas, Adição Subtração, Multiplicação, Divisão.

A adição, remove o ruído, pois por ele não estar em todas as imagens adicionados, a média some com esse outlier.

A subtração separa uma informação que interessa, ou seja, aquilo que é diferente de outra. Removendo por exemplo um fundo.

A multiplicação e divisão corrige sombras e níveis de cinzas irregulares.
A multiplicação também permite usar mascaras para apagar e preservar coisas de uma imagem.

Interseção, União, Complemento. E operações Lógicas, como And, Or, Xor e Not.

Transformações Espaciais Geométricas, é algo de Computação Gráfica.

Identidade, Escala, Translação, Rotação, Expansão e Contração (Warping, em que há se uma expansão ou seja aumentando um espaço, e contração diminuindo um espaço).

Dissolve, uma transição. Soma-se as imagens com porcentagens. (1-t)f + tg.

Ao juntar Warp com Dissolve, você cria o morph, que unifica as imagens, com o espaçamento e a cor.

Operações sobre pixeis individuais, ou seja, operações pontuais. transformação de intensidade para se obter o negativo. Para se borrar uma imagem, pode se usar mascaras, fazendo uma média.

O desvio padrão é uma boa estatística para identificar o contraste. 

Próxima Aula será prática.
