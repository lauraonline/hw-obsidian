Sistema hierárquico e distribuído para nomear dispositivos conectados à Internet ou a uma rede privada. Traduz URLs (ex: google.com) em [[Endereço IP|endereços IP]] (ex: 142.250.190.78).
## Funcionamento
1.  Usuário digita um URL no navegador.
2.  O sistema verifica o cache local pra ver se já tem o IP correspondente.
3.  Se não encontrado, envia uma consulta ao servidor DNS configurado.
4.  O servidor DNS procura o endereço IP correspondente.
5.  O endereço IP é retornado.
6.  O computador se conecta ao servidor pelo IP.
## Tipos de Servidores
* **Raiz**: Gerenciam os servidores TLD (.com, .net, .br, etc).
* **TLD**: Gerenciam os domínios de segundo nível (google.com, exemplo.com.br).
* **Autoritativos**: Mantêm os registros DNS de um domínio.
* **Recursivos**: Realizam a busca completa para o cliente.
## Registros DNS
* **A**: URL para [[Endereço IP#IPv4|IPv4]].
* **AAAA**: URL para [[Endereço IP#IPv6|IPv6]].
* **CNAME**: Alias conversor de um nome de texto simples para outro.
* **MX**: Servidores de email.
* **NS**: Servidores de nomes autoritativos.
* **TXT**: Informações de texto simples.