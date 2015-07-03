# Exercice 7

Calculate perimeter, area, volume, and diagonal of a parallelepiped.

Input: 
```
{Float} widthParallel
{Float} heightParalel
{Float} depthParallel
```

Output: 
```
{Float} perimeter
{Float} area
{Float} diagonal
{Float} volume
```

## Java implementation
```java
import java.util.Scanner;
public class Exercice07 {
  public static void main(String[] args){
    float width, height, depth, perimeter, area, volume, diagonal;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the width of the paralleleped:");
    width = input.nextFloat();

    System.out.println("Type de height of the paralleleped:");
    height = input.nextFloat();

    System.out.println("Type de depth of the paralleleped:");
    depth = input.nextFloat();

    perimeter = ( 2.0f * width + 2.0f * depth ) * 2.0f + 4.0f * height;
    area      = 2.0f * width * depth + 2.0f * width * height;
    volume    = width * depth * height;
    diagonal  = Math.sqrt( Math.pow( width, 2 ) + Math.pow( height, 2 ) + Math.pow( depth, 2 ) );

    System.out.println("Periemter: " + perimetro + "\n" + 
                       "Area: " + area + "\n" + 
                       "Volume: " + volume + "\n" +
                       "Diagonal: " + diagonal);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var width, height, depth, perimeter, volume, diagonal;

  width = prompt('Type the width of the parallelepiped:'); 
  width = parseFloat(width);

  height = prompt('Type the height of the parallelepiped:'); 
  height = parseFloat(height);

  depth = prompt('Type the depth of the parallelepiped:'); 
  depth = parseFloat(depth);

  perimeter = ( 2 * width + 2 * depth ) * 2 + 4 * height;
  area      = 2 * width * depth + 2 * width * height;
  volume    = width * depth * height;
  diagonal  = Math.sqrt( Math.pow( width, 2 ) + Math.pow( height, 2 ) + Math.pow( depth, 2 ) );

  alert('Perimeter: ' + perimeter + '\n' + 
        'Area: ' + area + '\n' + 
        'Volume: ' + volume + '\n' + 
        'Diagonal: ' + diagonal);
}());
```
