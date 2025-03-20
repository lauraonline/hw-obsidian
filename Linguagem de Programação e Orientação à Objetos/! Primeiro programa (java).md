## Convenções
- **Nome do projeto**: [[Camelcase]]
- **Nome de pacote**: Tudo minúsculo
- **Nome de classe**: [[Camelcase]]
## Comentários
Uma linha/inline: `\\`
Várias linhas: `\*` no começo e `*\` no final
## Hierarquia
### Pacotes
São como pastas que contém arquivos de código-fonte, usados para reunir classes semelhantes.
Fisicamente, ele só gera pastas dentro do sistema de organização de arquivos.
**Exemplo**: Pacote de gerenciamento de biblioteca
### Classes
É uma abstração de diferentes objetos semelhantes. Ela define o **comportamento** de seus objetos através de **métodos** e os **estados possíveis** destes objetos através de **atributos**.
**Exemplo**: Classe de livro, que representa qualquer livro e suas ações no sistema
### Objetos
Um objeto é uma instância única de uma classe. Ele é usado dentro de uma classe e tem atributos, como peso, nome, cor, e métodos, como andar, latir, etc.
**Exemplo**: Um livro específico (uma instância da classe Livro)
### Métodos
Ação que um objeto pode tomar. É um bloco de código que pode ser reutilizado chamando o método.
- Muito similar às funções do C++
**Exemplo**: Método pra fazer a retirada de um livro, método pra calcular multa por atraso de entrega, método em uma classe diferente pra pesquisar por um livro específico na biblioteca
### Exemplo
	package package1;
	public class Class01 {
		public static void main(String[] args) {
		System.out.println("Teste")
		}
	}
#### public
**Modificador** que torna a classe ou membro do projeto para todas as outras classes e pacotes do projeto.
#### main
**Método** que viabiliza a execução do programa. É executado apenas o que está dentro do método main.
#### static
Palavra-chave de objeto que indica que não precisa instanciar o objeto na memória. Não ocorre uso de construtor por fora do método main.
#### void
Palavra-chave de método pra fazer com que ele não dê um retorno.
### Delimitadores
**Ponto (`.`)**: Acesso a um membro de um objeto ou classe.
**Chave (`{}`)**: Determina o início e o fim de um método ou classe
**Colchete (`[]`)**: Determina o início e fim de um vetor
### Incremento e decremento
**Pós-incremento (`a++`)**: Adiciona 1 ao valor da variável após a execução da linha
**Pré-incremento (`++a`)**: Adiciona 1 ao valor da variável no momento de execução do comando
**Pós-decremento (`a--`)**: Subtrai 1 do valor da variável após a execução da linha
**Pré-decremento (`--a`)**: Subtrai 1 do valor da variável no momento de execução do comando
### Abreviação
`a += b` é o mesmo comando que `a = a + b`, só que abreviado
	A abreviação pode ser usada com qualquer operador **aritmético** (`+`, `-`, `*`, `/`, `%`)