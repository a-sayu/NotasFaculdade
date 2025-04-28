# Processamento Digital de Imagens

Tag: #3_Ano #PDI

---

Aula de hoje é sobre filtros.

---

Pega uma imagem transformada por Fourier, o filtro é como feito um produto, fazendo pixel a pixel, e aplicando a inversa de Fourier, teno uma imagem realçada.

![[FiltroPassaBaixaConceito.png]]

Filtragem no Domínio do Espaço x Filtragem no Domínio da Frequência(?)

Filtro Ideal é aquele que a função do filtro modifica de forma digital sem uma queda suave, e sim uma queda brusca.

A transformada de fourier guarda os valores em pouco espaço.

---

Filtro de Butterworth

O mais comum de filtros era ter uma curva, em que as frequências baicas são multiplicadas por valores grandes enquanto as frequencias mais altas eram multiplicados por frequências baixas.

Filtro Gaussiano

Que tem a curva normal, com uma função (depois eu copio aqui), terá um valor alto no meio e vai caindo conforme se afasta do "centro" da curva

Filtro Passa-Alta

Em que é invertido comparado a passa baixa, pois ele zera as baixas frequências, portanto bordas permanecem.

Filtros Butterworth Highpass

A altas frequências eram múltiplicadas por quase 1, por conta da curva analogica. tem uma equação que eu vou copiar depois

Filtro Gaussiano Highpass

![[FiltroPassaAltaGauss.png]]

---

Filtro High Boost

Em que se pega uma imagem com altas e baixas e soma as altas frequencias, fortalecendo a imagem original, se subtrair as baixas você tem só as altas, e ao somar as altas você tem uma imagem melhor.

Filtro Homomorphic

Trata a imagem como iluminação e reflectância, se tendo uma vantagem sobre os dois componentes, tendo como resultado uma imagem melhorada em partes mais escuras.

Uma aplicação muito importante para a filtragem do domínio, com um ruído periódico e de padrão, para filtrar ela e obtermos um espectro  de fofurier, teríamos uma baixa frequencia encontrada com pontos de valores altos em picos fora do espectro comum. 

Não implementaremos a Transformada de Fourier neste bimestre.

Fim do primeiro bimestre ---

Aula 7 estava prevista com outras transformadas, iremos implementar a transformada do cosseno, mas que talvez na proxima semana, ficaria-se a implementação devida na semana que vem.