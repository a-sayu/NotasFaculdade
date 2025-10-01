# 10.01 - Minicurso

## Tem slide

---

Complemento do Minicurso de Documentação e Produtividade com Markdown (Obsidian e GitHub)

Como utilizar o Git para sincronizar o Obsidian.

Instalar o Git.  

Acesse o [site do git-scm](https://git-scm.com/downloads) e selecione o seu sistema operacional.

![[Pasted image 20251001123415.png]]

Normalmente irá aparecer a versão indicada diretamente na telinha, no meu caso é o Windows.

![[Pasted image 20251001123528.png]]

Clique no primeiro link "Click here to download", que vai baixar a versão mais atualizada. Existem versões também que são de Instalador e Portáteis, a segunda sendo muito útil para usar com pendrives ou ambientes controlados.

![[Pasted image 20251001123817.png]]

Tendo o executável baixado, agora é só dar dois cliques no arquivo e instalar.

![[Pasted image 20251001123906.png]]

Clique em Executar e ele irá fazer a instalação do Git.

![[Pasted image 20251001124108.png]]

Clique em Next.

![[Pasted image 20251001124154.png]]

Clique em Next

![[Pasted image 20251001124240.png]]

Clique em Next.

![[Pasted image 20251001124302.png]]

Clique em Next.

![[Pasted image 20251001124432.png]]

A não ser que você tenha conhecimento prévio em Vim, prefira trocar por algo como o Nano ou Visual Studio Code. Clique em Next.

![[Pasted image 20251001124939.png]]

Defina como Override e Clique Next.

![[Pasted image 20251001125038.png]]

Clique em Next.

![[Pasted image 20251001125105.png]]

Clique em Next.

![[Pasted image 20251001125129.png]]

Clique em Next.

![[Pasted image 20251001125220.png]]

Clique em Next.

![[Pasted image 20251001125244.png]]

Clique em Next.

![[Pasted image 20251001125315.png]]

Clique em Next.

![[Pasted image 20251001125339.png]]

Clique em Next.

![[Pasted image 20251001125358.png]]

Clique em Install e esperar a instalação acabar.

![[Pasted image 20251001125614.png]]

Essa tela ira aparecer e iremos clicar na caixinha do Lauch Git Bash e depois Finish.

Configurar o Git

Para podermos usar o GitHub, precisamos configurar o Git, para isso na tela que temos agora aberta faremos os seguinte.

![[Pasted image 20251001125836.png]]

Ao inves de exemplo@email.com usaremos o email que você tem depois de cadastrar no github.

![[Pasted image 20251001130057.png]]

Ao inves de Fulano de Tal, troque pelo seu nome, não precisa ser o nome configurado no GitHub.

Feito isso, seu git está configurado, e iremos agora configurar para podemos utilizar o Obsidian para salvar as nossas anotações no GitHub.

![[Pasted image 20251001130730.png]]

Entre na pasta que você tem o seu Cofre do Obsidian, no meu caso está no `Downloads/CofreExemplo/` 

Para facilitar vou fazer a sequencia de comandos:

```git
git init                             ; inicializa o repositorio
git add .                            ; adiciona todas as alterações
git commit -m "mensagem do commit"   ; cria o commit das alterações
```

Agora teremos que criar um repositório no GitHub para armazenar nossas anotações:

![[Pasted image 20251001131514.png]]

No topo direito da tela, clique no `+`.

Salvar no Obsidian

![[Pasted image 20251001130308.png]]

Teremos essa tela, caso você tenha uma nota, feito alterações e etc.

![[Pasted image 20251001130339.png]]

Aqui deste lado é onde importa, iremos apertar na setinha com um circulo em volta

---

## ***log***

> *`upd`* : *note created -- month.day*