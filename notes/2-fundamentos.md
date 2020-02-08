## Web Moderno com JavaScript

### # Fundamentos

**Tipos de Dados:**

 * [var](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/var): 
 ao declarar uma variável com "var" é permitido que ela seja redeclarada posteriormente no código, 
 isto é, tendo o seguinte código:
 
    ```
    var a=10
    var a=20
    console.log(a)
    ```
    
    O valor impresso no console será 20, uma vez que esse valor foi redeclarado e a ele foi atribuido um novo valor.
    O valor da variável também pode sofrer mutações dentro de outros escopos:
    
    ```
    var a = 1;
    if (a >= 1) {
      var a = 4; // Declaração da variável dentro do escopo do bloco if

      console.log(a);  // Imprime 4
    } 
    console.log(a); // Imprime 4
    ```
    
    
  * [let](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/let): 
  
  * [const](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/const):