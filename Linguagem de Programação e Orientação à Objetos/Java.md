Linguagem de programação [[Linguagem orientada a objetos|orientada a objetos]] [[Linguagem compilada|compilada]] e [[Linguagem interpretada|interpretada]] desenvolvida pela Sun Microsystems (que foi comprada pela Oracle).
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
## Vantagens
- Portabilização: pode-se escrever um programa que será rodado em qualquer lugar que rode Java
- O encapsulamento de variáveis permite maior segurança
- Código organizado e claro
- Suporte ao Unicode
## Desvantagens
- Baixo desempenho quando comparada com linguagens não interpretadas, como C++
- Número grande de paradigmas e APIs que aumenta a barreira de entrada
- O código de máquina pode ser utilizado em processos de engenharia reversa, expondo o código-fonte
## Definições
- **.java**: Arquivo de código Java
- **Framework**: Biblioteca usada como base para o desenvolvimento de software
- **Javac**: Compilador de java
- **.class**: Arquivo de bytecode Java (compilado mas não interpretado)
- **[[#Java Virtual Machine (JVM)|Java Virtual Machine (JVM)]]**: Interpretador de java
- **[[Application Programming Interface (API)]]**: Bibliotecas de funções
- **Applets**: Pequenos aplicativos escritos em Java que rodam na JVM do browser.
## Java Runtime Environment (JRE)
É utilizado pra executar aplicativos feitos com Java. Contém a Java Virtual Machine (JVM) e bibliotecas utilizadas pra compilar o código-fonte.
## Java Virtual Machine (JVM)
Software que executa os aplicativos Java, traduzindo o bytecode (compilado) para código de máquina. Permite que o mesmo código Java possa ser executado em diversos computadores diferentes, dependendo apenas das limitações de hardware.
## JAR (.jar)
Extensão de arquivo compactado usado pra armazenar classes compiladas, arquivos diversos e metadados associados com um programa Java.
## Java Enterprise Edition (Java EE)
Plataforma de programação pra **servidores** com Java. 
- Contém bibliotecas desenvolvidas pra acesso a servidores, sistemas de e-mail, banco de dados, etc.
- Desenvolvido pra suportar uma grande quantidade de usuários ao mesmo tempo.
## Java Standard Edition (Java SE)
Plataforma de programação padrão pra Java. Contém o [[#Java Runtime Environment (JRE)|JRE]], as [[Application Programming Interface (API)|APIs]] do Java e outras ferramentas.
- Edição mais popular, geralmente utilizada pelos programadores iniciantes
- Voltada pra desenvolvimento para desktops e, secundariamente, servidores
## Java Micro Edition (Java ME)
Plataforma voltada pra desenvolvimento de aplicações **mobile** e de sistemas embarcados.
- Contém configurações e bibliotecas trabalhadas ao redor das limitações de hardware que vem com esses dispositivos