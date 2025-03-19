Mecanismo que permite que vários dispositivos em uma rede local ([[Local Area Network (LAN)|LAN]]) usufruam de um ou mais [[Endereço IP|endereços IP]] públicos para acessar a Internet.
## Função
* Economizar endereços IP públicos (especialmente [[Endereço IP#IPv4|IPv4]]), já que o número de endereços é limitado.
* Aumentar a segurança interna da rede, ocultando os endereços IP internos dos dispositivos da rede local.
## Tipos
* **Estático:** Mapeamento um-para-um entre um [[Endereço IP|endereço IP]] interno e um endereço IP público (cada IP interno tem seu próprio IP público previsível).
* **Dinâmico:** Mapeamento de um endereço IP interno para um endereço IP público de um pool de endereços disponíveis (cada IP interno tem um IP público aleatório).
* **PAT (Port Address Translation) ou NAT Sobrecarga:** Mapeamento de múltiplos endereços IP internos para um único endereço IP público, utilizando diferentes [[Porta (redes)|portas]] para distinguir as conexões (todo IP interno compartilha do mesmo IP público).
## Como Funciona
1. Um dispositivo na rede local envia um pacote para um destino na Internet.
2. O roteador NAT intercepta o pacote e substitui o [[Endereço IP|endereço IP]] de origem (interno) pelo endereço IP público do roteador.
3. O roteador NAT também altera a porta de origem do pacote e mantém uma tabela de tradução para rastrear a conexão.
4. O pacote é enviado para a Internet com o endereço IP público e a [[Porta (redes)|porta]] modificada.
5. Quando a resposta chega, ela é recebida pelo roteador NAT, que usa uma tabela de tradução para reverter as alterações e encaminhar o pacote para o dispositivo correto na rede local.
## Ver também
* [[Roteador]]
* [[Endereço IP]]