# Aula de Sistemas Operacionais

## Respondendo a questão 10 novamente por não ter guardado em algum local

10- Assim que o computador é ligado. Problema: você precisa descrever resumidamente cada uma das atividades que acontecem no computador da nossa empresa imediatamente após o computador ser ligado; você precisa saber quem é o principal responsável por essas atividades; e você deve deduzir onde o responsável por essas atividades fica armazenado.

**Resposta**: Verifica o setup, faz o POST, descompacta dados, lê dispositivos de armazenamento e carrega o sistema operacional; BIOS; ROM.

As etapas de inicialização do computador:

Na placa-mãe há um programa chamado BIOS que conta com as rotinas de E/S de baixo nível, ele fica em um flash RAM que não é volátil, mas que pode ser atualizado em caso de erros.

Quando um computador é incializado, o BIOS começa a executar, primeiro confere quanta RAM está instalada, se o teclado e outros dispositivos básicos estão instalados e respondendo corretamente.

Ele vê os barramentos PCI e PCIe para detectar dispositivos ligados a ele.

O BIOS determina o dispositivo de inicialização tentando uma lista de dispositivos armazenados na memória CMOS, se não inicializar através de uma unidade de CD-ROM/USB ele inicializa a partir do disco, no primeiro setor da memória contém um programa que examina a tabela de partições no final do setor de inicialização para determinar qual partição está ativa, então um carregador de inicialização secundário é lido daquela partição, lendo o sistema operacional da partição ativa e o inicia.
