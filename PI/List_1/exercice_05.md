# Exercice 5

Calculate perimeter, area and length of the diagonal of a square.

Input: 
```
{Float} squareBase
```

Output: 
```
{Float} perimeter
{Float} area
{Float} diagonal
```

## Java implementation
```java
import java.util.Scanner;
public class Exercice05 {
  public static void main(String[] args){
    float squareBase, perimeter, area, diag;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the of the square:");
    squareBase = input.nextFloat();

    perimeter = squareBase * 4.0f;
    area      = squareBase * squareBase;
    diag      = Math.sqrt( Math.pow( squareBase, 2 ) * 2.0f );

    System.out.println("Perimeter: " + perimeter + "\n" + 
                       "Area: " + area + "\n" + 
                       "Diagonal: " + diag);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var squareBase, perimeter, area, diagonal;

  squareBase = prompt('Type the base of the rectangle:'); 
  squareBase = parseFloat(squareBase);

  perimeter = squareBase * 4;
  area      = squareBase * squareBase;
  diagonal  = Math.sqrt( Math.pow(squareBase, 2) * 2 );

  console.log('Perimeter: ' + perimeter + '\n' + 
        'Area: ' + area + '\n' + 
        'Diagonal: ' + diagonal);
}());
```
