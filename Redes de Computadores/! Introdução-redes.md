## Componentes

![[Componentes1.png]]
1. Mensagem
	Informações sendo transmitidas (texto, números, figuras, áudio e vídeo)
2. Emissor
	Dispositivo remetente da mensagem
3. Receptor
	Dispositivo destinatário
4. Meio de transmissão
	Meio físico pelo qual a informação passa de um dispositivo para o outro (cabo de par trançado, coaxial, fibra ótica ou wireless: ondas de rádio)
5. [[Protocolo (redes)|Protocolo]]
	Conjunto de regras que controla e rege a transmissão
## Link
- Caminho de comunicação que transfere dados de um dispositivo a outro
- Velocidade da conexão é chamada de **largura de banda**
	- Medida em bits por segundo (bps, e.g. Gigabit)
## Modos de transmissão
### Fiação
- **Paralela**: 2 ou mais [[Bit|bits]] são enviados a cada [[Pulso de clock|pulso de clock]]
- **Serial**: Apenas 1 [[Bit|bit]] é enviado a cada [[Pulso de clock|pulso de clock]]
	- **Assíncrona**: O intervalo de tempo entre cada envio não é relevante, e tem um bit que determina o começo e o fim de uma divisão de dados
	- **Síncrona**: Os dados são enviados sem bits de início e fim, e o receptor faz o trabalho de separar a string contínua de informação e transformá-la numa mensagem legível
	- **Isócrona**: Os dados são enviados a uma taxa fixa e sincronizada (Ideal para áudio e vídeo em tempo real)
### Direção
![[Direção1.png]]
- **Simplex**: Transmissão de mão-única. Não há retorno do receptor. (Televisão, rádio, periféricos de computador como mouse, teclado)
- **Half-duplex**: Transmissão de mão-dupla não-simultânea. Há retorno do receptor, mas apenas depois do recebimento completo da mensagem do emissor.
- **Full-duplex**: Transmissão de mão-dupla simultânea. O meio pode ter dois caminhos (ida e volta), ou a capacidade do meio é dividida em dois canais que trafegam ambas as direções
## A Internet
![[Componentes2.png]]

## Modelo OSI (ISO)
### 7 camadas
1. Física
	Fluxo de [[Bit|bits]] em um meio.
	[[Hub (ethernet)|Hub]]
		Agrupa dispositivos em uma [[Local Area Network (LAN)|rede local]] de forma promíscua (sem inteligência).
	[[Network Interface Card (NIC)|Placa de rede (NIC)]]
		Lida com a conexão física cliente-rede
2. Enlace
	[[Endereço físico (MAC)]]
		Hexadecimal com 2 blocos de 24 bits cada, formando o endereço único de uma placa de rede.
	[[Ethernet]]
		Protocolo de transmissão de dados por rede. Pode usar cabos ou conexão sem fio (Wi-Fi).
	[[Switch]]
		Entrelaça diferentes dispositivos na mesma rede. Tem lógica para distinguir dispositivos pelos seus [[Endereço físico (MAC)|endereços físicos]]
		[[Network Address Translation (NAT)|NAT]]
			Mecanismo do switch que assinala endereços IP públicos a diferentes dispositivos na [[Local Area Network (LAN)|rede local]]
	[[Network Interface Card (NIC)|Placa de rede (NIC)]]
		Faz o endereçamento de um dispositivo para o switch ou roteador
3. Rede
	[[Roteador]]
		Interliga redes diferentes, como a rede local ([[Local Area Network (LAN)|LAN]]) e a internet ([[Wide Area Network (WAN)|WAN]])
	[[Endereço IP]]
		[[Endereço IP#IPv4|IPv4]]: 4 blocos de 8 bits cada, formando o endereço único de um dispositivo conectado a uma rede. (192.168.0.1)
4. Transporte
	[[Porta (redes)|Porta]]
		Ponto específico de conexão em um dispositivo de rede (switch, roteador, [[Network Interface Card (NIC)|NIC]]). Tem um número de 0 a 65535. 
5. Sessão
6. Apresentação
7. Aplicação
	Endereço URL
		Texto simples, que aponta para o endereço de um site com auxílio de uma tabela [[Domain Name System (DNS)|DNS]]
	[[Application Programming Interface (API)|API]]
		Estrutura que especifica como um programa deve solicitar informações a uma infraestrutura da Internet.
## [[TCP IP (protocolo)|TCP/IP]]
### 4 camadas
1. Enlace
	Camadas 1 e 2 do modelo OSI
2. Rede
	Camada 3 do modelo OSI
3. Transporte
	Camada 4 do modelo OSI
4. Aplicação
	Camadas 5-7 do modelo OSI
## Intranet
- Rede privada que usa a infraestrutura da Internet
- Não acessível a computadores externos
- Permite a utilização de serviços da internet, como e-mail, páginas web, [[File Transfer Protocol (FTP)|FTP]], etc.
## Extranet
- Método de conexão a uma Intranet por computadores externos
- Utilização de [[Virtual Area Network (VPN)|VPN]] para acesso
## Internet
- Rede pública de acesso geral
- Acessível a todos os computadores