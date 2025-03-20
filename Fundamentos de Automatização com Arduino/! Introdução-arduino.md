## [[Carga elétrica]]
**Propriedade elétrica** das partículas atômicas que compõem uma matéria. Medida em **Coulombs (C)**.
A matéria é dividida em elétrons, prótons e nêutrons.
### Carga elementar
É a carga elétrica de 1 elétron: 1,602 x10-19 C.
## [[Corrente elétrica]]
Taxa de **variação** da [[Carga elétrica]] em relação ao **tempo**.
- **Corrente elétrica contínua:** permanece constante e em uma direção
- **Corrente elétrica alternada:** varia senoidalmente com o tempo
![[AC vs DC1.png]]

O Arduino UNO lida somente com correntes elétricas contínuas.
## [[Tensão elétrica]]
A [[Corrente elétrica]] (ou seja, a energia em forma de elétrons) é movida de um lugar pro outro com a força da tensão elétrica, também conhecida como força eletromotriz (fem) ou diferença de potencial (DDP).
Ela é medida em Volts (V), e os volts representam a quantidade de energia necessária para mover uma unidade de [[Carga elétrica]] através de um elemento.
Ao lidar com Arduino, o termo mais comum para se referir à tensão elétrica é apenas "tensão".
## [[Potência]]
Qualquer circuito eletrônico é descrito pelas 3 grandezas [[Corrente elétrica|corrente]], [[Tensão elétrica|tensão]] e potência.
A potência dissipada por um resistor é calculada pela equação 
$$ P = V \times I $$ em que V é a corrente elétrica em Amps (A) e I é a tensão em Volts (V).
## Energia elétrica
É a somatória da potência elétrica durante o tempo em que um determinado circuito esteve em funcionamento. Obtida multiplicando a [[Potência|potência]] pelo tempo
- Medida em Joules (J) ou Watt-hora (Wh)
	A medida Watt-hora só pode ser calculada em casos que a potência é constante.
## Alimentando o Arduino UNO
O Arduino UNO é alimentado por um cabo **USB tipo B** ou uma fonte externa entre 6V e 12V. O circuito do Arduino contém reguladores que convertem a energia consumida pra 5V e 3V, dependendo da voltagem de entrada. A energia fornecida pelo Arduino para as portas de saída (I/O) varia entre 0V e 5V.
Ou seja, ao usar um componente externo (como um sensor) que trabalhe com 3.3V, é importante regular o nível de tensão externa do Arduino (de 5V pra 3.3V), para não queimar o pino do componente.
## [[Resistor|Resistores]]
Componentes que se opõem à passagem da corrente elétrica, ou seja, oferecem uma resistência.
É necessário um multímetro para medir a resistência, ou ler o [[Resistor#Código de cores|código de cores]].
