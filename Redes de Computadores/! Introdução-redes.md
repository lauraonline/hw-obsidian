## Componentes

![[{E188A13A-CA6F-443E-8B85-7366C9E1F659}.png]]
1. Mensagem
	Informações sendo transmitidas (texto, números, figuras, áudio e vídeo)
2. Emissor
	Dispositivo remetente da mensagem
3. Receptor
	Dispositivo destinatário
4. Meio de transmissão
	Meio físico pelo qual a informação passa de um dispositivo para o outro (cabo de par trançado, coaxial, fibra ótica ou wireless: ondas de rádio)
5. Protocolo
	Conjunto de regras que controla e rege a transmissão
## Modos de transmissão
### Fiação
- **Paralela**: 2 ou mais [[Bit|bits]] são enviados a cada [[Pulso de clock|pulso de clock]]
- **Serial**: Apenas 1 [[Bit|bit]] é enviado a cada [[Pulso de clock|pulso de clock]]
	- **Assíncrona**: O intervalo de tempo entre cada envio não é relevante, e tem um bit que determina o começo e o fim de uma divisão de dados
	- **Síncrona**: Os dados são enviados sem bits de início e fim, e o receptor faz o trabalho de separar a string contínua de informação e transformá-la numa mensagem legível
	- **Isócrona**: Os dados são enviados a uma taxa fixa e sincronizada (Ideal para áudio e vídeo em tempo real)
### Direção
![[{BE708EDD-CFFC-48D0-80C2-362875EF3ABC}.png]]
- **Simplex**: Transmissão de mão-única. Não há retorno do receptor. (Televisão, rádio, periféricos de computador como mouse, teclado)
- **Half-duplex**: Transmissão de mão-dupla não-simultânea. Há retorno do receptor, mas apenas depois do recebimento completo da mensagem do emissor.
- **Full-duplex**: Transmissão de mão-dupla simultânea. O meio pode ter dois caminhos (ida e volta), ou a capacidade do meio é dividida em dois canais que trafegam ambas as direções
## A Internet
![[{74F698CF-640B-4706-A290-64C79C99CDBC}.png]]

## Modelo OSI (ISO)
### 7 camadas
1. Física
	Fluxo de [[Bit|bits]] em um meio.
2. Enlace
	[[Endereço físico (MAC)]]
		Hexadecimal com 2 blocos de 24 bits cada, formando o endereço único de uma placa de rede.
	[[Ethernet]]
	[[Switch]]
		[[Network Address Translation (NAT)|NAT]]
3. Rede
	[[Roteador]]
		Interliga redes diferentes, como a rede local ([[Local Area Network (LAN)|LAN]]) e a internet ([[Wide Area Network (WAN)|WAN]])
	[[Endereço IP]]
		[[Endereço IP#IPv4|IPv4]]: 4 blocos de 8 bits cada, formando o endereço único de um dispositivo conectado a uma rede. (192.168.0.1)
4. Transporte
	[[Porta]]
		
5. Sessão
6. Apresentação
7. Aplicação
	Endereço URL
		Texto simples, que aponta para o endereço de um site com auxílio de uma tabela [[Domain Name System (DNS)|DNS]]
## Modelo TCP/IP
### 4 camadas
1. Enlace
	Camadas 1 e 2 do modelo OSI
2. Rede
	Camada 3 do modelo OSI
3. Transporte
	Camada 4 do modelo OSI
4. Aplicação
	Camadas 5-7 do modelo OSI