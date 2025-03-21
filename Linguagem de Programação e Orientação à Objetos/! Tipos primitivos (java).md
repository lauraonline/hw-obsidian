## Tipos
Tipos primitivos de variáveis:
- `int`
	Números inteiros.
	**Tamanho**: 4 [[Byte|bytes]]
	**Alcance**: de -2.147.483.648 a 2.147.483.647 
- `long`
	Números inteiros grandes.
	**Tamanho**: 8 [[Byte|bytes]]
	**Alcance**: de -9.223.372.036.854.775.808 a 9.223.372.036.854.750.000
- `short`
	Números inteiros pequenos.
	**Tamanho**: 2 [[Byte|bytes]]
	**Alcance**: de -32768 a 32767 
- `byte`
	Números inteiros muito pequenos. 
	**Tamanho**: 1 [[Byte|byte]]/8 [[Bit|bits]]
	**Alcance**: de -128 a 127
- `float`
	Números reais (fracionados).
	**Tamanho**: 4 [[Byte|bytes]]
	**Alcance**: de 3.4e-38 a 3.4e38
- `double`
	Números reais calculados com maior precisão.
	**Tamanho**: 8 [[Byte|bytes]]
	**Alcance**: de 1.7e-308 a 1.7e308 
- `char`
	Um caractere Unicode.
	**Tamanho**: 4 [[Byte|bytes]]
	**Alcance**: de \u0000 (0) a \uffff (65.535)
- `boolean`
	Uma condição (true ou false).
	**Tamanho**: 1 [[Bit|bit]]
	**Alcance**: de 0 (false) a 1 (true)
## Casting
Ato de denotar o tipo de variável com qual interpretar o valor de uma variável.
**Por exemplo**:
`float salario 2543.79F` Por padrão, o compilador prefere que esse valor fosse atribuído a uma variável `double`, mas colocando F na frente do número, ele sobrepõe o padrão.
 Similarmente, pode-se escrever da maneira `float salario (float) 2543.79`, e terá o mesmo efeito.
 Essa técnica pode ser utilizada pra "forçar" tipos menores a aceitar valores maiores, como fazer um valor long caber numa variável int, mesmo que seja grande demais, mas isso não é recomendado.
## String
**NÃO** é um tipo primitivo. String é uma **classe**, e ao ser declarada, deve ter a primeira letra maiúscula (`String`).
É usada pra armazenar cadeias de caracteres.
- Pode ser usada igual uma variável primitiva, com exceção da capitalização
- Não tem limite de tamanho
## Ver também
- [[Java#Casting]]