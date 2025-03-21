## Operador ternário
Usado pra atribuir um resultado de if/else a uma variável.
Sintaxe: `condicao ? verdadeiro : falso`.
Por exemplo:
```
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
```
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
## Ver também
- [[Java#Operador ternário]]
- [[Java#Switch]]