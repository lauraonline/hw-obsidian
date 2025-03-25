Declarados com uma forma de referência com a forma de objeto atribuída. Por exemplo:
```java
public static void main (String[] args) {  
    int[] idades = new int[3];
    idades[0] = 15;  
    idades[1] = 21;  
    idades[2] = 25;
}
```
Alternativamente, pode-se usar chaves (`{}`) pra preencher o array automaticamente.
```java
public static void main (String[] args) {  
    int[] idades = {15,21,25};  
}
```
Valores padrão:
- byte, short, int, long, double: `0`
- char: `'\u0000'`, ou `' '`
- boolean: `false`
- String: `null`
## Redeclaração
Pode-se redeclarar o array com (exemplo: array com nome `frases` e tipo `String`) `frases = new String[5];`. O tamanho do array redeclarado pode ser qualquer um, e ao redeclarar, o array antigo é deletado e não pode ser recuperado.
## Foreach
Forma do `for` especializada pra imprimir arrays por completo. Por exemplo:
```java
public static void main (String[] args) {  
    int[] numeros2 = {1,2,3,4,5};  
    for (int i : numeros2) {  
        System.out.println(i);  
    }  
}
```
Dentro dos parâmetros do for, basta declarar um incrementador do mesmo tipo do array e colocar um `:`. Depois, é só colocar o nome do array.
Ao imprimir, é importante imprimir o incrementador, não o array com o índice do incrementador.
## Arrays multidimensionais
Arrays que fazem referência a outros arrays.
![[Array multidimensional1.png]]
```java
public static void main (String[] args) {  
    int[][] numeroDiasTrimestres = new int[4][3];  
    numeroDiasTrimestres[0][0] = 31;  
    numeroDiasTrimestres[0][1] = 28;  
    numeroDiasTrimestres[0][2] = 31;
    // ...
    numeroDiasTrimestres[3][0] = 31;
    numeroDiasTrimestres[3][1] = 30;  
    numeroDiasTrimestres[3][2] = 31;  
}
```
### Array base
Array que serve como referência para outros arrays. Seu conteúdo (e tipo) é um endereço de memória, que aponta pra cada array respectivo.
#### Foreach (arrays multidimensionais)
Ao usar o foreach em um array base, é necessário que o tipo do array seja um vetor. Por exemplo:
```java
public static void main (String[] args) {  
    int[][] numeroDiasTrimestres = new int[4][3];  
    numeroDiasTrimestres[0][0] = 31;  
    // ...
    numeroDiasTrimestres[3][2] = 31;  
    for (int[] base:numeroDiasTrimestres) {  
        for (int i:base) {  
            System.out.println(i);  
        }  
    }  
}
```
No loop do array base, o tipo do incrementador é `int[]`, e o array base é usado como array de referência no loop seguinte.
## Inicialização
Ao inicializar um array, não é preciso inicializar os arrays não-base. Dessa maneira, pode-se fazer com que os arrays não-base tenham tamanhos variados. Por exemplo:
```java
public static void main (String[] args) {  
    int[][] arr1 = new int[3][];  
    arr1[0] = new int[2];  
    arr1[1] = new int[3];  
    arr1[2] = new int[4];  
}
```
![[ArrayMultidimensionalTamanhosDiferentes1.png]]
### Chaves
O array multidimensional pode ser preenchido usando chaves também, de duas maneiras:
```java
public static void main (String[] args) {  
    int[][] arr1 = new int[3][];  
    arr1[0] = new int[]{1, 2};
    arr1[1] = new int[]{1, 2, 3};  
    arr1[2] = new int[]{1, 2, 3, 4};  
} // Ao contrário de um array unidimensional, é necessário inicializar e declarar o tipo de array antes de preencher os valores entre as chaves, com new int[].
```

```java
public static void main (String[] args) {  
    int[][] arr2 = {{1, 2}, {1, 2, 3}, {1, 2, 3, 4}};  
}
```
## Propriedades
`[nome-do-array].length`: retorna o tamanho do array
## Ver também
- [[Java#Arrays]]