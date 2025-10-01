# 10.01 - Minicurso

## Complemento do Minicurso de Documentação e Produtividade com Markdown (Obsidian e GitHub)

Como utilizar o Git para sincronizar o Obsidian.
### Instalar o Git.  

Acesse o [site do git-scm](https://git-scm.com/downloads) e selecione o seu sistema operacional.

![[Pasted image 20251001123415.png]]

---

Normalmente irá aparecer a versão indicada diretamente na telinha, no meu caso é o Windows.

Clique no primeiro link "Click here to download", que vai baixar a versão mais atualizada. Existem versões também que são de Instalador e Portáteis, a segunda sendo muito útil para usar com pendrives ou ambientes controlados.

![[Pasted image 20251001123528.png]]

---

Tendo o executável baixado, agora é só dar dois cliques no arquivo e instalar.

![[Pasted image 20251001123817.png]]

---

Clique em Executar e ele irá fazer a instalação do Git.

![[Pasted image 20251001123906.png]]

---

Clique em Next.

![[Pasted image 20251001124108.png]]

---

Clique em Next

![[Pasted image 20251001124154.png]]

---

Clique em Next.

![[Pasted image 20251001124240.png]]

---

Clique em Next.


![[Pasted image 20251001124302.png]]

---

A não ser que você tenha conhecimento prévio em Vim, prefira trocar por algo como o Nano ou Visual Studio Code. Clique em Next.

![[Pasted image 20251001124432.png]]

---

Defina como Override e Clique Next.

![[Pasted image 20251001124939.png]]

---

Clique em Next.

![[Pasted image 20251001125038.png]]

---

Clique em Next.

![[Pasted image 20251001125105.png]]

---

Clique em Next.

![[Pasted image 20251001125129.png]]

---

Clique em Next.

![[Pasted image 20251001125220.png]]

---

Clique em Next.

![[Pasted image 20251001125244.png]]

---

Clique em Next.

![[Pasted image 20251001125315.png]]

---

Clique em Next.

![[Pasted image 20251001125339.png]]

---

Clique em Install e esperar a instalação acabar.

![[Pasted image 20251001125358.png]]

---

Essa tela ira aparecer e iremos clicar na caixinha do Lauch Git Bash e depois Finish.

![[Pasted image 20251001125614.png]]

---

### Configurar o Git

Para podermos usar o GitHub, precisamos configurar o Git, para isso na tela que temos agora aberta faremos os seguinte.

Ao inves de exemplo@email. com usaremos o email que você tem depois de cadastrar no github.

![[Pasted image 20251001125836.png]]

---


Ao inves de Fulano de Tal, troque pelo seu nome, não precisa ser o nome configurado no GitHub.

Feito isso, seu git está configurado, e iremos agora configurar para podemos utilizar o Obsidian para salvar as nossas anotações no GitHub.

![[Pasted image 20251001130057.png]]

---

Entre na pasta que você tem o seu Cofre do Obsidian, no meu caso está no `Downloads/CofreExemplo/` 

![[Pasted image 20251001130730.png]]

Para facilitar vou fazer a sequencia de comandos:

```git
git init                             ; inicializa o repositorio
git add .                            ; adiciona todas as alterações
git commit -m "mensagem do commit"   ; cria o commit das alterações
```

Agora teremos que criar um repositório no GitHub para armazenar nossas anotações:

No topo direito da tela, clique no `+`.

![[Pasted image 20251001131514.png]]

---

Clique em New repository

![[Pasted image 20251001174702.png]]

---

Para ter consistência, vamos nomear com o mesmo nome do nosso Cofre, em seguida colocamos como privado para acesso somente nosso e colocamos sem README, criando clicando no botão verde abaixo.

![[Pasted image 20251001174757.png]]

---

Copia o link clicando nos quadrado com quadrados dentro.

![[Pasted image 20251001174922.png]]

---

Ai vocês colam o seguinte comando no git bash:

```
git remote add origin https://github.com/a-sayu/CofreExemplo.git
```

E em seguida envia:

```
git push -u origin main
```

![[Pasted image 20251001180724.png]]

---

E pronto! Se você olhar, as suas notas estaram no github.

![[Pasted image 20251001180752.png]]

---
### Salvar no Obsidian

![[Pasted image 20251001175435.png]]

Teremos essa tela, caso você tenha uma nota, feito alterações e etc.

![[Pasted image 20251001175606.png]]

E é esse pedacinho que importa, pois ta vendo aquela seta dentro do circulo, você não tera mais que se preocupar com terminal git e etc, você pode só apertar ele, e tudo irá para o github.

Se quiser algo automático, nas configurações (engrenagem), em seguida git (ao final da barra de navegação vertical nos plugins não oficiais)

![[Pasted image 20251001175948.png]]

E você altera o 0 para um outro número, que vai representar quantos minutos até ele atualizar sozinho e o segundo da commit apenas se você parar de editar o arquivo.

É isso, espero que vocês se divirtam! Se precisarem de qualquer coisa, me enviem um e-mail ou mesmo um toque no instagram (@sayu_abi) ou discord (sayu.sayu).

---

## ***log***

> *`upd`* : *note created -- 10.01*