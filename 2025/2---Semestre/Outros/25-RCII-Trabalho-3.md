## 1.1 Introdução

> *Apresentar uma **introdução** sobre o problema de loops em redes Ethernet e a importância dos protocolos Spanning Tree.*
> 
> *Finalize com uma frase de transição, mostrando que nas próximas seções serão abordados o funcionamento e as diferenças entre os protocolos.*

Um loop de rede ocorre quando ocorre uma conexão entre duas portas de uma tomada de rede, essa ligação cria um loop de rede ethernet, esse tipo de ocorrência pode ser acidental ou intencional, em caso de necessidade de conferir falhas na infraestrutura da rede.

Este tipo de ocorrência deve ser feitas cautela pois esse tipo de ocorrência apresenta alguns problemas que afetam o desempenho da rede:

- **Broadcast storm**, onde quadros de broadcast seriam retransmitidos de forma excessiva na rede, pois os switches retransmitem quadros em broadcast através de suas demais portas, e quando há um caminho fechado, os quadros são retransmitidos continuamente pelos switches, inundando a rede, e consumindo a sua capacidade.
- **Instabilidade na tabela MAC nos switches**, cada switch tem uma tabela que mapeia endereços físicos MAC de dispositivos para as portas correspondentes em um switch, essa tabela então indica a porta por onde um quadro deve ser retransmitido para que seja transmitido para seu endereço MAC de destino. Como essa tabela é dinâmica, ela é constantemente atualizada e sobrescrita criando conflitos.
- **Múltiplos quadros repetidos recebidos em cada host**, cada quadro recebido também tem que ser processado, e isso cria um peso para o equipamento final no tempo de processamento desses quadros repetidos.

Afim de impedir que loops em redes façam de circular pacotes continuamente foi criado o protocolo STP, ou Protocolo Spanning Tree, que soluciona o problema de loops em redes LAN, conferindo a redundância na rede, bloqueando alguns caminhos garantindo que os dados se movam eficientemente.

Nas próximas seções desse trabalho serão tratados de forma mais aprofundada os protocolos STP, RSTP e MSTP, conceitos fundamentais para compreensão do funcionamento e entendimento dos protocolos, a arquitetura de rede proposta para a segunda parte do trabalho e o plano de endereçamento IP e VLANs definidas.

## 1.2 Protocolos STP, RSTP e MSTP

> *Descrever o **funcionamento do STP, RSTP e MSTP**, destacando suas diferenças, vantagens e limitações.*
> 
> *Apresente um **quadro comparativo** com os três protocolos (tempo de convergência, suporte a VLANs, complexidade, padrões IEEE, etc.).*

Como apresentado anteriormente, o protocolo STP foi desenvolvido para resolver problemas de redundância em redes ethernet, sendo um protocolo padrão aberto e que impede broadcast storms, instabilidade da tabela MAC, loops e quadros multiplos repetidos. Desde o seu desenvolvimento ocorreram atualizações: Rapid STP, ou RSTP e Multiple STP, ou MSTP que melhoraram o STP.

### 1.2.1 STP
### 1.2.2 RSTP
### 1.2.3 MSTP
## 1.3 Conceitos Fundamentais

> *Explicar os **conceitos fundamentais**:*
> 
> - *Root Bridge*
> - *Port States (Blocking, Listening, Learning, Forwarding)*
> - *Bridge ID e Path Cost*
> - *Eleição e convergência da topologia*

## 1.4 Objetivos Gerais e Específicos

Os objetivos deste trabalho estão divididos em um objetivo geral e pbjetivos específicos, conforme descritos a seguir.

### 1.4.1 Objetivo Geral

Projetar e configurar uma rede corporativa de médio porte utilizando STP, RSTP e MSTP, analisando seu comportamento, tempos de convergência e desempenho em situações de falha.

### 1.4.2 Objetivos Específicos

- Compreender o funcionamento dos protocolos STP, RSTP e MSTP.
- Criar uma topologia de rede redundante em laboratório ou ambiente de produção.
- Implementar e comparar os três protocolos em cenários distintos ou iguais.
- Medir o tempo de convergência e estabilidade da rede (mesmo em redes simuladas).
- Propor boas práticas para ambientes corporativos com múltiplas VLANs (item não obrigatório).

## 1.5 Arquitetura de Rede Proposta

*Apresentar uma **arquitetura de rede proposta** com a quantidade de equipamentos (switches e computadores) e suas funções.*

*Descreva a topologia geral (quantidade de switches, hosts, servidores, etc.).*

*Indique funções dos dispositivos (core, distribuição, acesso).*

*Inclua um diagrama de rede (mesmo que conceitual).*

## 1.6 Endereçamento de IP e Esquema de VLANs

*Elaborar um **endereçamento IP e esquema de VLANs** adequado ao projeto. (item não obrigatório)*

*Mostre o plano de endereçamento IP e as VLANs definidas.*

*Explique a lógica de segmentação (por setor, função, departamento, etc.).*

*Pode incluir uma tabela com IPs, máscaras, VLAN IDs e descrições.*

https://www.pynetlabs.com/spanning-tree-protocol-explained/
https://www.tp-link.com/br/support/faq/3898/
https://glmtec.com.br/entenda-o-loop-de-rede-e-como-preveni-lo/
https://www.cisco.com/c/pt_br/support/docs/lan-switching/spanning-tree-protocol-stp-8021d/221722-troubleshoot-mac-flaps-loop-on-cisco-cat.html?utm_source=chatgpt.com
https://moodle3.ifsc.edu.br/mod/book/view.php?id=312208&chapterid=56881&lang=pt_br