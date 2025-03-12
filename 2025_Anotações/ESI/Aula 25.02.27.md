# Engenharia de Software I

Tag: #ES #ESI
## Gerenciamento de Configuração.

A atividade que entrelaça todas as atividades de Desenvolvimento. E é essencial para garantir a qualidade e acompanhamento de alterações.

* Identificar Alterações
* Controlar Alterações
* Assegurar que as alterações estão implementadas corretamente
* Relatar as alterações a outro interessados

Essas alterações parecem pouco mas ocorrem tanto em Definição, Desenvolvimento e Manutenção, e quem deve fazer a comunicação dessas alterações é o Gerenciamento de Configuração.

Configurações tem Itens, que devem ser selecionados, eles podem ser um Produto de Software ou Produto de Desenvolvimento de Software que é escolhido.

P Software: Qualquer coisa que vai ser entregue à um usuário final, documentação também, mas não é entregue.

O gerenciamento de configuração fornece a memória de um produto. Que permite por exemplo encontrar modificações, o que é muito importante para muitos em um mesmo produto.

Tarefas que o GC ajuda:

1. Identificação
2. Controle de Mudanças
3. Controle de Versão
4. Auditoria de Configuração
5. Relato de Situação
6. Controle de Interface
7. Controle de Subcontratados e Fornecedores

Conceitos Fundamentais

Baseline (Linha de Referência): É a verificação antes de sair para um ponto, a fim de corrigir para a entrega para esse ponto, a partir do momento que passar da baseline, tem que ter varias pessoas concordando.
Repositório dos Itens de Configuração: Um lugar para colocar todos os itens.
Check In / Check Out: Método de controle na entrada e saída do repositório.

Baseline:
* Ponto de Progresso Mensurável
* Base para o Desenvolvimento e Controle Subsequente
* Ponto de Medida para avaliar Qualidade

Em uma cascata é fácil de observar as baselines, que fica no final de cada etapa. Itens de Configuração que passou pela linha básica, ele é congelado, não deve mais ser mexido (baselined). Para voltar, para algo antigo, é muitas coisas para voltar, custando tempo e dinheiro.

Quando eu baixo um item de configuração (copio) em um local, criando uma alteração nesse item, em que se ele não estiver congelado, não há problema em retornar, passado da baseline, isso não pode ser aceito tão facilmente.

Cada item de configuração deve ser: Identificado, Analisado, Corrigido e Aprovado.

Itens de Configuração só podem ser alterados após uma solicitação aprovada por todos.

Check Out, é a cópia localmente de um repositório, ao realizar a cópia:
* Marcar que algo foi copiado, quem e todo o controle: Permissões, Avisos.

Check In, é a volta com a versão modificada da cópia:
* Desbloquear o que foi bloqueado, ou seja que não está mais sendo alterado, anotar também o controle: Quem pegou, quem alterou e quando alterou.

Tasks de Gerenciamento de Configuração:
1. Tarefas Preliminares:
	* Selecionar o que irá ser um item.
		* Qualquer item relevante: Mais usados, Genéricos, Importantes, (?), (?)
		* Evitar Super Documentação
	* Descrever os itens a serem selecionados.
		* (Classes de Relacionamento)
	* Planejar as linhas de referência, um bom ponto é o final de uma fase.
	* Descrever a maneira em que eles serão arquivados e recuperados.
2. Identificação
3. Controle de Mudança: 
	* Quem dá acesso, quem pode fazer mudanças (burocracia de controle)
	* Principalmente: Prioridade de Pedidos
4. Controle de Versão: 
	* Controle de Alterações no repositório.
	* Uma árvore que utiliza ou Delta Negativo ou Delta Positivo.
		* Negativa: Guarda a mais recente e as diferenças existentes até então. Ele não vai ter o código anterior e sim o mudou de: para:
		* Positiva: Guarda a mais antiga e todas as variações, é um custo maior.
5. Auditoria: 
	* Funcional: Verificar se está funcionando. Atividade de Controle de Qualidade, Encontrar Omissões (por exemplos de atividades que deveriam ter sido feitas) ou Erros.
	* Física: Complementa com questões de ações aprovadas, confirmações, revisões técnicas formais, padrões de engenharia seguidos, data, autor, procedimentos de administração, itens de configuração relacionados formam atualizados apropriadamente?
6. Relato de Situação:
	* O que aconteceu, quem fez, e o que mais está sendo afetado.
7.  Controle de Interface: Coordenar mudanças, Descrever tipo de interface, organizacionais afetadas, não de software. Como documento são aprovados (burocracia).
8. (Ler depois)

Ferramentas de GCS para auxiliar as atividades de gerenciamento de configuração de software:
* exemplos de repositório antigos local:
	* CVS
	* RCS
	* SCCS
	* VersionWeb
	* Subversion
* Atuais:
	* Gitlab
	* Github
	* Etc.

Git Flow (Conjunto de Slides contando o que acontece)

Branch: Galhos, ramificações.
Hotfix: Check Out > Correção Rápida (Cliente e Dev) > Check In.

Homologação: Burocracia da Organização. Homologado é uma operação com a autorização de alguém.