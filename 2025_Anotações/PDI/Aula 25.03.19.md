# Aula de PDI

Tag: #3_Ano #PDI 

Realce no Espaço

Realce é melhorar uma imagem com alguma finalidade específica, portanto fazer um processamento para essa finalidade.

Duas formas de processamento, a partir de uma operação pontual ou por operação baseada em vizinhança.

***
Pontual
Um ponto me interessa a cada momento.

G(x,y) = T[f(x,y)]

Exemplo de Transformações T.

Binarização
Em que abaixo de um tom será 0, e acima de outro será 1. Importante notar que o usuário que define como será a transformação.

Imagens Negativas
* Imagens Médicas
* Construção de Slides a partir de negativos de filmes fotográficos
* Evidenciar características não percebidas na imagem positiva.

> *r é o tom original da imagem

Compressão de Escala Dinâmica
Utiliza transformações logarítmicas, que conseguem melhorar a as quantidades de valores de formas mais claras.
* S = c . log(1+r)

Funções Potências
Vários dispositivos se captura impressão e visualização operam com respostas lineares.
* S = c . r ^ y ou S = c . ( r + e ) ^ y

Função de Transformação Linear por partes
Se pode dar uma esticada nas cores para encontrar resultados agradáveis.

Fatiamento de Tons de Cinza
É possível criar funções que atendem uma especificação, portanto selecionando o que se deseja.

Fatiamento de planos de bits
Imagine uma imagem, se eu pegar um determinado pixel, e ele é um byte, o primeiro bit define se ele é claro ou escuro, e o último demonstra o fino detalhe. Muitas vezes é possível remover bits de pouca importância para se ter uma imagem que ocupa menos espaço.

Processamento de histograma, estatística da imagem
Ele conta a frequência de tons que se tem em uma imagem. Para ser analise para um computador, não importa muito a localização de tons, mas para o olho humano é importante.

Equalização de Histogramas
Em que em uma imagem original, faz se uma operação pixel a pixel, tenha um histograma bem distribuído.

Você pega todos os pontos, e calcula a frequência de cada tom, em seguida faz a frequência acumulada de cada tom. O valor então é calculado da seguinte maneira:

máximo[ 0, round((tons_cinza * freq_acumulada)/(col * lin)) -1 ]

**Prática para final de Bimestre: equalização de imagens**

Todos os trabalhos estão dentro de um único ambiente.

Especificação de Histogramas
A equalização apenas garante o espaçamento adequado das cores, portanto é possível processar a imagem no sentido de atender um certo histograma estabelecido previamente

Equalização de histogramas local
Propõe-se que se obterá um histograma apenas ao redor de um pixel, para cada pixel vc olha a vizinhança dele e se obtém um resultado "melhor".

Mascaras AND e OR

Subtração de Imagens
Demonstra a diferença entre as imagens, obtendo um contraste.

Media de Imagens
Ele permite a remoção de ruído, pois ruido é algo aleatório, pois ele some na soma permitindo que ele perca por não ser grande coisa. É possível também usar uma mediana, portanto pegando só o que está no meio.

***
Operação baseada em vizinhança

Filtragem Espacial - Mascara de Convolução
A convolução de duas funções é uma integral, em que ela irá calcular uma área entre essas curvas, a cada momento.

Convolução em Imagens
Somatória da multiplicação com um filtro g, deslocando um único pixel até chegar no último

Filtro da Média
* Filtro passa baixa
Ele calcula a média, somando 5 pixels e divide por 5, sendo a vizinhança-4, é possível também usar a vizinhança-8, suavizando imagens, eliminando ou atenuando ruídos. Em efeito colateral, a imagem fica borrada.

Filtro da Mediana
É mais interessante, pois a média pode estourar por conta de valores fora do comum, a mediana vai pegar o que está ao meio de uma ordenação do pixel e da vizinhança-8 e selecioná-lo.

Prática: Implementar filtro de Média e Mediana. Com 10% de ruído sal e pimenta.

```
tamanho = largura*altura;
nruido = tamanho/10
for i = 1 to nruido do
	begin
		x = random(largura);
		y = random(altura);
		c = random(1); ----> 0 ou 1
		if c = 1 then c = 255
			Ins[x,y] = c;
	end
```

