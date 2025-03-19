Identificador único atribuído a uma placa de rede (NIC) para comunicação em uma rede local ([[Local Area Network (LAN)|LAN]]).
* 2 blocos de 24 [[Bit|bits]] (48 bits, 6 bytes)
* Representado em hexadecimal (ex: 00:1A:2B:3C:4D:5E)
* Os primeiros 24 bits identificam o fabricante da placa (OUI - Organizationally Unique Identifier)
* Os últimos 24 bits são atribuídos pelo fabricante ao dispositivo específico
* Usado na camada de enlace do [[! Introdução-redes#Modelo OSI (ISO)|modelo OSI]]
## Função
* Identificar unicamente um dispositivo na rede local
* Usado para encaminhar pacotes de dados dentro da [[Local Area Network (LAN)|LAN]]
* Utilizado no protocolo Ethernet
## Como Encontrar
* **Windows:** `ipconfig /all` (procure por "Endereço Físico")
* **Linux/macOS:** `ifconfig` ou `ip addr` (procure por "ether" ou "link/ether")