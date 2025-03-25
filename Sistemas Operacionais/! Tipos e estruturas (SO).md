## Tipos de SOs
### Monoprogramados (ou monotarefas)
Só permitem um programa ativo de uma vez, que ocupa a RAM até ser fechado.
- Enquanto o programa em questão estiver aberto, **todos** os recursos do SO são dedicados a ele.
	Por isso que só dá pra usar um de cada vez
**Exemplos:**
- MS-DOS
- Terminal (SO simulado)
	Prompt de comando no Windows, Terminal em outros SOs
#### Sistemas Batch (lote)
Consiste em submeter o sistema a vários processos (programas) de uma só vez (em lote), de forma sequencial (ordenada). Dessa maneira, o sistema executa todos os processos na ordem em que foram requisitados.
Enquanto o lote (sequência) de programas estiver sendo processado, não há interação do usuário com o sistema.
### Multiprogramados (ou multitarefas)
Mantém mais de um programa na memória, compartilhando o tempo de CPU e outros recursos do PC com eles
- Há várias tarefas ao mesmo tempo, no mesmo processador: enquanto uma é processada, a outra espera a vez dela.
- Requer que o processador tenha mecanismos de troca rápida de processos

#### Sistemas interativos
Permitem que o usuário interaja com o sistema no meio do processo.
#### Sistemas de tempo compartilhado
Permitem ser controlados por vários usuários ao mesmo tempo. Enquanto a tarefa do usuário 1 está sendo processada, o tempo de CPU excedente (não usado) é alocado pra tarefa executada pelo usuário 2, e por aí vai.
#### Sistemas de tempo real
Cada tarefa tem um tempo pré-determinado (prazo), e o sistema é instruído a concluir a tarefa nesse tempo. Se ele consegue concluir a tarefa nesse prazo, já é outra história...
##### Rígido (ou crítico, ou *hard*)
Tem comportamento determinístico, ou seja, o sistema **precisa** concluir a tarefa no prazo.
Por exemplo, freio ABS: se o sistema não corrigir o padrão de frenagem a tempo, o carro pode derrapar e machucar alguém.
##### Leve (ou moderado, ou *soft*)
Se o processo não terminar a execução no prazo, ele pode continuar executando até terminar. No caso, o prazo é apenas uma sugestão.
Por exemplo, um aparelho DVD: é desejável que ele comece a ler o disco em 2 segundos, mas se ele demorar mais, não vai causar nenhum dano grave.
## Estruturas de SO
### Monolítica
O sistema operacional é um único módulo (o núcleo), que contém todas as funções e serviços que usam o hardware pra executar as aplicações.
- As aplicações usam [[System call|system calls]] pra fazer requisições pro SO.
### Micronúcleo (microkernel)
Torna o núcleo do SO o menor possível. Assim, o máximo de operações do SO são realizadas fora dele. Dessa maneira, as aplicações podem usar as funções e serviços pra interagir com o hardware de maneira oposta ao sistema monolítico.
### Camadas
O sistema se torna **modular**, pra ter melhor reusabilidade e ser menos complexo, e **hierárquico**, o que significa que a cada nível de operação, os detalhes das operações dos níveis inferiores podem ser ignorados.
**Por exemplo**:
- Nível 1: núcleo
- Nível 2: entrada e saída básicos
- Nível 3: gerenciamento de memória
- Nível 4: sistema de arquivos
- Nível 5: compilador de linguagem de programação
	Cada nível precisa dos níveis inferiores pra funcionar, mas você não precisa se preocupar com o nível 1 pra executar uma tarefa nível 2, e por aí vai.
### Máquina virtual
Consiste em fazer [[System call|system calls]] pra o que as aplicações vêem como um sistema (ou vários sistemas), que na verdade é um sistema emulando outro (ou emulando vários).
#### [[Java#Java Virtual Machine (JVM)|Java Virtual Machine (JVM)]]
Máquina virtual em formato de software que executa os aplicativos Java, traduzindo o bytecode (aplicativo compilado) para código de máquina. Permite que o mesmo código Java possa ser executado em diversos computadores diferentes, dependendo apenas das limitações de hardware.
	Um sistema pode emular uma JVM, e o aplicativo verá apenas a JVM e o que o sistema permitir ser passado pra JVM