# Exercice 4

Calculate perimeter, area and length of the diagonal of a rectangle.

Input: 
```
{Float} rectBase
{Float} rectHeight
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
public class Exercice04 {
  public static void main(String[] args){
    float rectBase, rectHeight, perimeter, area, diagonal;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the base of the rectangle:");
    rectBase = input.nextFloat();

    System.out.println("Type the height of the rectangle:");
    rectHeight = input.nextFloat();

    perimeter = rectBase * 2.0f + rectHeight * 2.0f;
    area      = rectBase * rectHeight;
    diagonal  = Math.sqrt( Math.pow(rectBase, 2) + Math.pow(rectHeight, 2) );

    System.out.println("Perimeter: " + perimeter + "\n" + 
                       "Area: " + area + "\n" +
                       "Diagonal: " + diagonal);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var rectBase, rectHeight, perimeter, area, diagonal;

  rectBase = prompt('Type the base of the rectangle:'); 
  rectBase = parseFloat(rectBase);

  rectHeight = prompt('Type the height of the rectangle:'); 
  rectHeight = parseFloat(rectHeight);

  perimeter = rectBase * 2 + rectHeight * 2;
  area      = rectBase * rectHeight;
  diagonal  = Math.sqrt( Math.pow(rectBase, 2) + Math.pow(rectHeight, 2) );

  console.log('Perimeter: ' + perimeter + '\n' + 
        'Area: ' + area + '\n' + 
        'Diagonal: ' + diagonal);
}());
```
