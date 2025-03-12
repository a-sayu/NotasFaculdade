# Cores

Tag: #PDI

Luz Branca

Teoria da cores Tricromaticas.

Modelo de Cores Aditivo

Modelo de Cores Subtrativos
Utilizado em impressoras, a soma de Ciano, Magenta e Amarelo resulta em Preto.

Representação de Imagens Digitais Coloridas
Normalmente, há três sensores que capturam informação e três canais de cor (RGB), cada pixel é um vetor 3x1.

Dentro desses sensores, um ponto máximo é branco, significando o uso total da cor, portanto, mais claro, maior uso.

As imagens são representadas em matriz, e dentro dessa matriz cada local representa um pixel da imagem.

**Não é comum, e não usaremos, mas** outra forma pode ser através de paleta de cores, em que ao salvar a imagem, é necessário salvar a paleta de cores, utilizando um índice na tabela da paleta de cores.

Cada pixel pode ter associado a ele uma quantidade de bits que é dividido entre os canais de cores RGB. O verde normalmente recebe maior quantidade de bits, pela maior sensibilidade ao verde.
* 16 bits (R: 5, G: 6, B: 5)
* 24 bits (R = G = B: 8 bits -> true color)
* 32 bits (true color + canal alfa: 8 bits -> transparência)

Nada mais é do que a quantização, ou seja, o número de níveis ao digitalizar algo. Mas a maior quantidade de bits, maior a amostragem, maior a resolução.

Dithering, uma técnica muito usada em impressoras, para se conseguir imagens maiores, sendo usado no caso de ter poucas cores, a fim de ter mais tons. Ele anexa pixeis criando cores.

Uma transição de vermelho para preto, escurecendo o vermelho (v: vermelho, p: preto)
vv/vv -> vv/vp -> vv/pp -> vp/pp -> pp/pp

Distinção das Cores
* Brilho/brightness - noção acromática de intensidade
* Matiz/hue - atributo relacionado a cor (onda) dominante
* Saturação/saturation - pureza de uma cor

HSV, é o modo que possui a distinção das cores.
Matiz e Saturação compões a cromaticidade.

Diagramas de Cromaticidade
É como se pegasse um objeto 3D e cortasse para formar a figura das cores, observando principalmente o comprimento da onda, basicamente aplanando as cores para o 2D.

* No centro o branco. Na curva externa há as cores puras, a matiz.
A cor dominante é definida indo do ponto A até o branco em linha reta, e onde cruzar na borda do diagrama, é a cor dominante, sendo o comprimento de onda da cor.
Cores complementares, seria aquela que ao passar por A até o branco, em linha reta, a mesma quantidade ao lado oposto, encontrando uma cor B.

Modelos de Cor
Especificar um sistema coordenadas onde cada ponto representa uma cor diferente.

Monitor Colorido RGB
Cada canal é quantizado em 8 bits, há 16 milhões de cores no RGB, cubo solido de cores (Aditivo). Quando a quantidade é igual para cada canal, se tem tons de cinza.

Equação da luminância

I = 0,299R + 0,587G + 0,114B -> Cinza mais interessante ao olho humano
Dando um peso maior para o verde, de modo simplificado é só fazer a média.

Impressão Colorida CMY e CMYK (K = Preto)
É também um cubo solido de cores, mas que a soma de todos seria preto (Subtrativo)
Ele é baseado nas cores secundárias, a conversão CMY para RGB ou o contrário, supondo valores normalizados (as cores dentro de uma faixa, normalizados entre 0 e 1, se a faixa for de 0 a 255, o 1 seria na verdade 255).

C = 1 - R
M = 1 - G
Y = 1 - B

Na teoria, C=M=Y=1 geram a cor preta, na pratica cria um verde escuro.

R = 1 - C
G = 1 - Y
B = 1 - M

Interpretação Visual HSI - intensidade (HSV - value, HSL - luminosity, sempre no terceiro uma intensidade)

Modelo YIQ, na década que criaram a Televisão, só havia um tom de brilho, preto/branco, mandando todas as cores de pixel. Na época, se mandava apenas 1 informação, o tom de cinza, e depois de um tempo surgiu a TV colorida, para manter a compatibilidade, iriam continuar enviando a informação do cinza e a televisão moderna também iria receber o tom de cinza + as informações coloridas.

Modelo usado pela TV NTSC

Y: Intensidade
I, Q: Componentes de Cromaticidade
RGB x A (Matriz com luminância e outros) para se obter YIQ

Modelo YUV, similar ao YIQ, que era valores diferentes embaixo na matriz (os outros). Modelo usado para TV PAL. Ou seja, a luminosidade estaria certa, so mudaria a forma de conversão das cores.

Modelo YCbCr

Modelo HSI, se entendia que para o olho humano, era melhor identificar as cores do que identificar o RGB, que precisaria mexer em diversas cores para reconhecer cores. Entretanto, a distância euclidiana entre vetores não reproduzem fielmente a diferenças de cores. Ele desacopla a informação de intensidade e informação cromática.

****

HSV - HSI - HSL são muito similares, voltados ao usuário, pensando em um círculo ou um cone.

H: geralmente um ângulo (360º, ou uma normalização 0-100, 0-255)

