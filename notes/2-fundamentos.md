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
 ao declarar uma variável com "let", diferentemente da variável "var", só é possível redeclara-lá posteriormente se a mesma estiver em um escopo diferente do bloco de código, como mostra o exemplo abaixo:
  
    ```
    let x = 1;

    if (x === 1) {
      let x = 2;
      console.log(x);  // Imprime 2
    }
    
    console.log(x); // Imprime 1
    ```
Os valores obtidos do no console são diferentes pois cada um possui seu escopo, onde um não interfere no outro.    
  
  * [const](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/const):
ao declarar uma variável "const" o seu valor não pode ser alterado, uma vez que isso ocorra, um erro acontecerá. Variáveis "const" são usadas para valores que não tem a necessidade de alteração durante a execução de um código, como, por exemplo:
  
  ```
  function calcularCircunferencia(raio) {
    const pi = 3.141592653589793;
    return 2 * pi * raio;
  }

  console.log(calcularCircunferencia(10)); // Imprime 62.83185307179586
  ```
  
  Ao calcular a circunferência de um círculo, o valor de PI permanece inalterável, deste modo, ele é uma constante.
  
