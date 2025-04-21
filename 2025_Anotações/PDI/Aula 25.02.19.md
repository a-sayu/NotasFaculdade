# Processamento Digital de Imagens

Tags: #3_Ano #PDI 

---

Esta aula foi apresentação da disciplina, anotações iniciais do caderno repassadas para o digital.

Livro: Digital Image Pocessing, 2ed.

⭐ Rede Neural Convolucional (.. )
⭐ Processamento Digital de Imagens é aplicável à vídeos também? 
⭐ Redes CNN (.. )

**Avaliaçâo:**
$Nota_1 = 0.8 * Prova 1 + 0.2 * Trabalhos$
$Nota_2 = 0.8 * Prova 2 + 0.2 * Trabalhos$
Se $Nota_1 + Nota_2 < 12$ então realizar prova 3
$Nota_3 = Prova 3$
$Media Final = \frac{(Nota_1 + Nota_2 + 2 . Nota_3)}{4} > 5$  

---

## Conteúdo

**Fundamentos de Imagens Digitais:**
- Elementos de Percepção Visual
- Estrutura do olho humano
- Formação de imagem no olho
- Sensibilidade do olho

**Representação de Imagens:**
- Teoria de Sinais
- Paradigmas de Abstração: níveis de Abstração, discretização e reconstrução, codificação e decodificação.
- Modelos matemáticos de sinais: aproximação de sinais, modelos funcionais e níveis de abstração
- Teoria de amostragem: amostragem pontual e uniforme
- Modelo de imagem
- Amostragem e Quantização
- Relações entre pixels: vizinhança, conectividade, medidas de distância

**Transformada de Fourier:**
- Introdução a Transformada de Fourier
- Transformada discreta de Fourier
- Algumas propriedades da Transformada bi dimensional de Fourier
- Teorema da amostragem de Shannon-Whittaker
- Transformada rápida de Fourier

> *É interessante pois ela sai do domínio da imagem e vai para o domínio da frequência, onde é mais fácil de realizar algumas operações*

**Realce de Images:**
- Operações Pontuais
- Realce por processamento pontual
- Transformação por intensidade
- Manipulação de histograma
- Subtração de imagem
- Filtragem espacial
- Fundamentos: Convolução
- Filtros de suavização
- Filtros de realce de altas frequências

> *Operações para melhorar a qualidade das imagens, isto é, nítida para uma pessoa, mais bonita de se ver, restauração de imagens. A subtração por exemplo é simples, significa subtrair de uma imagem outra imagem, podendo reconhecer diferenças entre imagens, utilizada para muitas aplicações como reconhecimento de desmatamento.*

**Fundamentos de Cor e Sistemas de Representação:**
- O Universo Físico de cor: formação das cores
- O Universo Matemático de cor
- O Universo de representação de cor: sistemas refletivos de cor, sistemas emissivos de cor
- Representação CIE-RGB: experimentos de comparação de cor
- Sólido de cor: espaço de cromaticidade
- Mudança de cor entre sistemas
- Sistemas de cores complementares
- Sistemas de interface de cor: Sistema IHS
- Mudançã entre os sistemas RGB
- Realce no domínio da cor

> *Entendimento de cor, nós da computação utilizamos dois modelos de cores: RGB em monitores, o branco se olhado bem próximo é o pixel vermelho, verde e azul no máximo, CMY em impressoras, Ciano, magenta e amarelo, ao imprimir se é feita a conversão da tela RGB para CMY.*

**Restauração de Imagens:**
- Transformações Geométricas
- Interpolação de níveis de cinza

> *Veremos tecnicas de restauração de imagem para que ela fique melhor, por exemplo proporção, borramento ou esticamentos sofridos*

**Compreessão de Imagens:**
- Fundamentos
- Modelos de compressão de imagens
- Compressão livre de erro
- Compressão com perdas
- Codificação por transformadas

> *Exemplos de compressão: JPEG, entendendo os modelos, se pode pensar nas tecnicas para guardar em arquivos menores, afim de minimizar o desperdício de espaço com repetições, transformadas de fourier e cosseno são métodos de compactação de imagem*

**Segmentação de Imagens:**
- Operações baseadas em bordas
- Afinamento de bordas
- Limiarização
- Transformada de Hough
- Crescimento de Regiões

> *Segmentar significa repartir a imagem em partes, bordas são muito importantes para reconhecer separações entre areas, Limiarização é o uso de um limiar, que é um número que reconhece a diferença entre dois valores resutando em um limiar para separação de uma area para outra para por exemplo binarizar uma imagem, Hough: encontrar objetos/retas/circulos na imagem*

**Representação e Descrição:**
- Chain Code, Aproximação Poligonal, Assinatura, Fecho Convexo, Esqueletos, Descritores de Fronteira, Números de Formas, descritores de Fourier, Descritores Regionais, Descritores Topológicos, Descritores baseados em Textura, Momentos, Matrizes de Co-ocorrência

> *Descrição: usa-se descritores, características para as imagens, medidas sobre a imagem. É útil para reconhecimento e diferenciação de itens em imagens, encontrar bons descritores é importante, por isso há vários descritores, atualmente as redes CNN são interessantes para que ao colocar as imagens nas redes ela própria começa a extrair números sobre essas diferenciações e itens*

**Morfologia:**
- Introdução
- Operadores Morfológicos

> *Segmentação de imagens, realce de imagens, muitos usos*

---
## Processamento Digital de Imagens

As imagens que vamos processar são digitais e o processamento também é digital portanto é o processamento digital de imagens digitais.
## Áreas Relacionadas

![[PDI.png]]

Iremos fazer além de processamento de imagens também a extração de dados e medidas.

**Origem**:
- Industria de Jornais transportando uma imagem por um cabo submarino entre Nova York e Inglaterra.

Através de sensores eles olhavam a imagem e do outro lado reconstruiam a imagem com outra máquina.

**Aplicações**:
- Radiação
- Sons
- Modelamento e Visualização

Espectro eletomagnético possui o comprimento da onda, sendo o visível minúsculo.

(.. 🚧 00:41:28 🚧 ..)

---

**Camera de Satélite:**

![[CameraSatelite.png]]

---

![[Pasted image 20250420154317.png]]

---

Uma imagem pode ser definida como uma função bidimensinoal f(x,y), onde x e y sâo coordenadas espaciais e a amplitude de f é chamada instensidade da imagem no local, se x,y e amplitude são valores finitos e discretos, diz-se que a imagemé digital. Caso contrário é analógico.

Processamento de Imagem define uma nova image em termos da que já existe.

```

g(x,y) = T(f(x,y))

g --> Imagem de saída
T() --> Operação de Transformação
f --> Imagem de Entrada

```

- Realce de Contraste

---
