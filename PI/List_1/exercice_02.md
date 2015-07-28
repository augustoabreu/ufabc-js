# Exercice 2

Calculate quotient and remainder of a division between two numbers.

Input: 
```
{Float} divisor
{Float} dividend
```

Output: 
```
{Float} rest
{Float} quotient
```

## Java implementation
```java
import java.util.Scanner;
public class Exercice02 {
  public static void main(String[] args){
    float divid, divis, quotient, rest;

    Scanner input = new Scanner(System.in);

    System.out.println("Type a number:");
    divid = input.nextFloat();

    System.out.println("Type another number:");
    divis = input.nextFloat();

    quotient  = divid / divis;
    rest      = divid % divis;

    System.out.println("Dividend: " + divid + "\n" +
                       "Divisor: " + divis + "\n" +
                       "Quotient: " + quotient + "\n" +
                       "Rest: " + rest);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var divid, divis, quotient, rest;

  divid = prompt('Type an number:'); 
  divid = parseFloat(divid);

  divis = prompt('Type another number:'); 
  divis = parseFloat(divis);

  quotient  = divid / divis;
  rest      = divid % divis;

  console.log('Dividend: ' + divid + '\n' + 
        'Divisor: ' + divis + '\n' +
        'Quotient: ' + quotient + '\n' +
        'Rest: ' + rest);
}());
```
