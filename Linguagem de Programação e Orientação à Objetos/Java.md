*Desenvolva uma vez, execute em qualquer lugar*
Linguagem de programação [[Linguagem orientada a objetos|orientada a objetos]] [[Linguagem compilada|compilada]] e [[Linguagem interpretada|interpretada]] desenvolvida pela Sun Microsystems (hoje Oracle).
## História
Em 1991, na Sun Microsystems, em Mountain View, CA, foi iniciado o **Green Project**, um projeto de planejamento de uma linguagem orientada a objetos. A ideia era fundamentar uma linguagem que pudesse unir lógica entre computadorxes e aparelhos domésticos.
### StarSeven
A primeira invenção da equipe foi o StarSeven (`*7`).
- Controle remoto em formato de TV com interface touchscreen
- Tinha um "mascote" que ensinava o usuário a usar
Inicialmente foi programado em C++ entre outras linguagens, mas nenhuma satisfazia as demandas da equipe, então foi criada uma linguagem nova, que seria:
- Pequena e eficiente
- Facilmente portável
- Simples de entender
### Oak
James Gosling, um dos engenheiros da Sun, criou e nomeou a linguagem de programação a ser utilizada no StarSeven. O nome escolhido foi **Oak**
Ao ver que o nome Oak já estava sendo usado, a Sun decidiu escolher o nome **Java**.
O nome originou de um tipo de café, produzido na ilha de Java, na Indonésia.
### HotJava
Navegador criado em 1994, feito completamente em Java com o propósito de rodar [[Java#Applet|applets]] Java.
### Java Development Kit (JDK)
Kit básico de desenvolvimento Java distribuído pela Sun (hoje Oracle) desde 1996. Contém uma coleção de ferramentas de programação feitas pra programar com Java, como
- [[Java#Java Runtime Environment (JRE)|Java Runtime Environment (JRE)]]
	Software utilizado pra compilar e rodar programas Java no computador.
- Um compressor de código que comprime o programa em um arquivo JAR.
e muitas outras ferramentas de desenvolvimento.
DIsponibilizado em versões [[#Java Enterprise Edition (Java EE)|EE]], [[#Java Standard Edition (Java SE)|SE]] e [[#Java Micro Edition (Java ME)|ME]]
![[JDK1.png]]
## Aplicações
- Serviços financeiros
- Marketing e propaganda
- Jogos multiplayer e salas de chat
- Educação
- Telefonia
- Lógica para sistemas embarcados
### Vantagens
- Portabilização: pode-se escrever um programa que será rodado em qualquer lugar que rode Java
- O encapsulamento de variáveis permite maior segurança
- Código organizado e claro
- Suporte ao Unicode
### Desvantagens
- Baixo desempenho quando comparada com linguagens não interpretadas, como C++
- Número grande de paradigmas e APIs que aumenta a barreira de entrada
- O código de máquina pode ser utilizado em processos de engenharia reversa, expondo o código-fonte
## Ambiente Java
### Java Runtime Environment (JRE)
É utilizado pra executar aplicativos feitos com Java. Contém a Java Virtual Machine (JVM) e bibliotecas utilizadas pra compilar o código-fonte.
### Javac
Compilador de Java incluído no JRE. Com o comando `javac [Arquivo .java]`, pode transformar arquivos .java em .class (bytecode a ser interpretado pela JVM)
### Java Virtual Machine (JVM)
Software que executa os aplicativos Java, traduzindo o bytecode (compilado) para código de máquina. Permite que o mesmo código Java possa ser executado em diversos computadores diferentes, dependendo apenas das limitações de hardware.
### JAR (.jar)
Extensão de arquivo compactado usado pra armazenar classes compiladas, arquivos diversos e metadados associados com um programa Java.
### Java Enterprise Edition (Java EE)
Plataforma de programação pra **servidores** com Java. 
- Contém bibliotecas desenvolvidas pra acesso a servidores, sistemas de e-mail, banco de dados, etc.
- Desenvolvido pra suportar uma grande quantidade de usuários ao mesmo tempo.
### Java Standard Edition (Java SE)
Plataforma de programação padrão pra Java. Contém o [[#Java Runtime Environment (JRE)|JRE]], as [[Application Programming Interface (API)|APIs]] do Java e outras ferramentas.
- Edição mais popular, geralmente utilizada pelos programadores iniciantes
- Voltada pra desenvolvimento para desktops e, secundariamente, servidores
### Java Micro Edition (Java ME)
Plataforma voltada pra desenvolvimento de aplicações **mobile** e de sistemas embarcados.
- Contém configurações e bibliotecas trabalhadas ao redor das limitações de hardware que vem com esses dispositivos
## Convenções
- **Nome do projeto**: [[Camelcase]]
- **Nome de pacote**: Tudo minúsculo, começando com o nome do website da empresa invertido. Exemplo: uk.lauraonline.devdojojava
- **Nome de classe**: [[Camelcase]]
- **Nome de variável**: Primeira letra minúscula, depois, [[Camelcase]]
## Comentários
**Uma linha/inline**: `//`
**Várias linhas**: `/*` no começo e `*/` no final
**Javadoc (várias linhas)**: `/**` no começo e `*/` no final
## Casting
Ato de denotar o [[! Tipos primitivos (java)#Tipos|tipo de variável]] com qual interpretar o valor de uma variável.
**Por exemplo**:
`float salario 2543.79F` Por padrão, o compilador prefere que esse valor fosse atribuído a uma variável `double`, mas colocando F na frente do número, ele sobrepõe o padrão.
 Similarmente, pode-se escrever da maneira `float salario (float) 2543.79`, e terá o mesmo efeito.
 Essa técnica pode ser utilizada pra "forçar" tipos menores a aceitar valores maiores, como fazer um valor long caber numa variável int, mesmo que seja grande demais, mas isso não é recomendado.
## Hierarquia
### Pacotes
São como pastas que contém arquivos de código-fonte, usados para reunir classes semelhantes.
Fisicamente, ele só gera pastas dentro do sistema de organização de arquivos.
**Exemplo**: Pacote de gerenciamento de biblioteca
### Classes
É um "molde" feito pra criar diferentes objetos com características em comum. Ela define o **comportamento** de seus objetos (ações em que eles podem participar) através de **métodos** e os **estados possíveis** destes objetos (dados atribuídos a eles) através de **atributos**.
**Exemplo**: Classe `Item`, que representa qualquer item na biblioteca e suas ações no sistema
### Subclasses
São classes "filhas" que herdam características das classes "mães", como classes Carro e Moto que herdam características em comum da classe Veículo.
**Exemplo**: Classe `Livro`, que é filha da classe "item" e representa um de qualquer livro da biblioteca
#### Objetos
Um objeto é uma instância única de uma classe. Ele é usado dentro de uma classe e tem atributos, como peso, nome, cor, e métodos, como andar, latir, etc.
**Exemplo**: Um livro específico (uma instância da classe `Livro`)
##### Atributos
Dados específicos sobre um objeto, que descrevem características ou estados do mesmo. Podem ser de vários tipos de dados, e podem ser públicos ou privados.
**Exemplo**: Estado do livro (No acervo ou sendo emprestado), número de páginas, número de vezes que foi emprestado, etc.
##### Métodos
Ação que um objeto pode tomar. É um bloco de código que pode ser reutilizado chamando o método.
- Muito similar às funções do C++
**Exemplo**: Método pra fazer a retirada de um livro, método pra calcular multa por atraso de entrega, método em uma classe diferente pra pesquisar por um livro específico na biblioteca
## Conceitos
- **.java**: Arquivo de código Java
- **Framework**: Biblioteca usada como base para o desenvolvimento de software
- **.class**: Arquivo de bytecode Java (compilado mas não interpretado)
- **Applets**: Pequenos aplicativos escritos em Java que rodam na JVM do browser.
### Encapsulamento
Técnica que envolve proteger os atributos e métodos sensíveis/confidenciais de uma classe e expor uma interface controlada pra interagir com a classe.
Em Java, consiste em tornar atributos sensíveis privados (palavra-chave `private`), para que só possam ser acessados de dentro da própria classe, e usar getters e setters pra obter o valor de um atributo e modificá-lo respectivamente.
### Herança
Conceito que consiste em uma classe ser baseada em outra classe mais abrangente. Por exemplo, uma superclasse (ou classe mãe, ou classe base) `Veículo`, que tem atributos como `marca`, `modelo` e `ano` pode ter seu código reutilizado em uma subclasse (ou classe filha, ou classe derivada) `Carro`, ou `Moto`, que tem atributos mais específicos.
### Polimorfismo
Capacidade de uma mesma ação (método) de ser realizada por diferentes objetos de diferentes classes. Por exemplo, um método que qualquer objeto que pertença à superclasse `Veículo` (como um objeto de `Carro` ou `Moto`) pode executar, como `Vender`.
## Operador ternário
Usado pra atribuir um resultado de if/else a uma variável.
Sintaxe: `condicao ? verdadeiro : falso`.
Por exemplo:
```java
public static void main (String[] args) {  
    float salario = 6000F;  
    String mensagemComprarPlay5 = "Vou comprar um PS5";  
    String mensagemNaoComprarPlay5 = "Não tenho condições de comprar um PS5";  
    String resultado = salario > 5000 ? mensagemComprarPlay5 : mensagemNaoComprarPlay5;  
    System.out.println(resultado);  
}
```
Caso a `condicao` seja verdadeira, o valor em `verdadeiro` será atribuído à variável. Caso contrário, o valor em `falso` será atribuído.
## Switch
Usado pra condicionar várias ações ao valor de uma variável.
Por exemplo:
```java
public static void main (String[] args) {  
    byte numeroDiaDaSemana = 4;  
    String nomeDiaDaSemana = null;  
    switch (dia) {  
        case 1:  
            nomeDiaDaSemana = "domingo";  
        case 2:  
            nomeDiaDaSemana = "segunda";  
        case 3:  
            nomeDiaDaSemana = "terça";  
        case 4:  
            nomeDiaDaSemana = "quarta";  
        case 5:  
            nomeDiaDaSemana = "quinta";  
        case 6:  
            nomeDiaDaSemana = "sexta";  
        case 7:  
            nomeDiaDaSemana = "sábado";  
    }  
    System.out.println("Dia da semana:" + nomeDiaDaSemana);  
}
```
Caso a variável (`dia`) tenha o valor em `case` (1-7), o código dentro do case será executado.
## Break e continue
O break faz com que o compilador salte pra fora de qualquer estrutura de repetição.
Por exemplo:
```java
public static void main (String[] args) {  
    int valorMax = 50;  
    for (int i = 1; i <= valorMax; i++) {  
        if (i > 25) {  
            break;  
        }  
        System.out.println(i);  
    }  
}
```
Mesmo que o `for` faça com que o `i` vá até 50, por causa da condicional `if (i > 25)`, quando o `i` for maior que 25, ele ativa o `break` e sai do loop antes de imprimir.

O continue com que o compilador pule uma iteração no loop, e continue depois dela.
Por exemplo:
```java
public static void main (String[] args) {
	for (int i = 1; i <= 10; i++) {
	  if (i == 4) {
	    continue;
	  }
	  System.out.println(i);
	}
}
```
O for conta os números de 1 até 10, mas pula o número 4. 
## Arrays
Declarados com uma forma de referência com a forma de objeto atribuída. Por exemplo:
```java
public static void main (String[] args) {  
    int[] idades = new int[3];
    idades[0] = 15;  
    idades[1] = 21;  
    idades[2] = 25;
}
```
Valores padrão:
- byte, short, int, long, double: `0`
- char: `'\u0000'`, ou `' '`
- boolean: `false`
- String: `null`
**Ver também:** [[! Arrays#Foreach|Foreach]], [[! Arrays#Propriedades|Propriedades]]
### Arrays multidimensionais
Compostos por arrays base, que contém endereços de memória dos sub-arrays.
**Ver também:** [[! Arrays#Foreach (arrays multidimensionais)|Foreach (arrays multidimensionais)]], [[! Arrays#Inicialização|Inicialização]]