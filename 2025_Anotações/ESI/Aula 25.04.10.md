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
- Atributo: Existe por apenas um tempo, necessária para uma aplicação significativa, sendo necessária o registro, sendo a maneira mais comum, se devendo as associações. Para quem ele quiser mandar algo, ele deve ter um atributo apontando para o objeto que ele quer se comunicar. Em que a associação vira um atributo que tem que enxergar outra classe.
- Parâmetro: 
- Localmente Declarada:


---