# Atividade 2 - B1

De acordo com a teoria da atividade 1 - B1, desenvolva em python 3.8.x+ um cookie e coloque no servidor 146.235.33.66.

Este cookie deve conter as seguintes características:
1. Nome e Valor
	- Nome (chave) identifica o cookie
	- Valor que armazenar, como o contador, ID de sessão e idioma
2. Validade / Expiração (expires ou max-age)
	- Controla a duração do cokie.
	- Essencial para diferenciar:
		- Duração até fechar o navegador (se não definir expires).
		- Duração até um tempo definido (7 dias, 30 dias).
3. Tentar identificar o tema = escuro do navegador;
	- Data ou hora da última visita;
	- Timestamp da visita (Exemplo: visitado em)
	- Origem da visita (Exemplo: Referencia = Google)
	- Tipo de Navegador/Sistema Operacional
