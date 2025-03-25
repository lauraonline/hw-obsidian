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
    switch (numeroDiaDaSemana) {  
        case 1:  
            nomeDiaDaSemana = "domingo";  
            break;  
        case 2:  
            nomeDiaDaSemana = "segunda";  
            break;  
        case 3:  
            nomeDiaDaSemana = "terça";  
            break;  
        case 4:  
            nomeDiaDaSemana = "quarta";  
            break;  
        case 5:  
            nomeDiaDaSemana = "quinta";  
            break;  
        case 6:  
            nomeDiaDaSemana = "sexta";  
            break;  
        case 7:  
            nomeDiaDaSemana = "sábado";  
            break;  
        default:  
            nomeDiaDaSemana = "erro";  
            break;  
    }
```
Caso a variável (`dia`) tenha o valor em `case` (1-7), o código entre o case e o break será executado. Caso **nenhum** case satisfaça o valor da variável, o código entre o `default`e o break será executado.
## Ver também
- [[Java#Operador ternário]]
- [[Java#Switch]]