## Break
Faz com que o compilador salte pra fora de qualquer estrutura de repetição.
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
## Continue
Faz com que o compilador pule uma iteração no loop, e continue depois dela.
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