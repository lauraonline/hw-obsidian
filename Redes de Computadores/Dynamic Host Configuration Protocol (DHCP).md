Protocolo de rede que atribui automaticamente [[Endereço IP|endereços IP]] e outros parâmetros de configuração de rede a dispositivos em uma rede.
## Ciclo
1. Um dispositivo (cliente) envia uma solicitação DHCP (DHCP Discover) para a rede.
2. Um servidor DHCP recebe a solicitação e oferece um endereço IP disponível (DHCP Offer).
3. O cliente aceita o endereço IP oferecido (DHCP Request).
4. O servidor DHCP confirma a atribuição do endereço IP ao cliente (DHCP ACK).
5. O cliente passa a utilizar o endereço IP atribuído por um determinado período de tempo (lease time).
	- Na metade do lease time, o cliente tenta fazer a renovação do endereço IP com o servidor que o forneceu o IP.
	- Caso ela falhe, o cliente tenta de novo aos 87.5% do tempo, dessa vez transmitindo o pedido a todos os servidores DHCP disponíveis.
	- Caso os dois passos falhem, o cliente retoma o passo 1 para obter um novo endereço IP.
## Vantagens
*   Configuração automática de endereços IP, evitando conflitos.
*   Gerenciamento centralizado de endereços IP.
*   Facilidade de adicionar ou remover dispositivos da rede.
## Ver também
*   [[Endereço IP]]