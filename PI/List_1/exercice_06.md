# Exercice 6

Calculate perimeter, area of a circle.

Input: 
```
{Float} circleRadius
```

Output: 
```
{Float} perimeter
{Float} area
```

## Java implementation
```java
import java.util.Scanner;
public class Exercice6 {
  public static void main(String[] args){
    float circleRadius, perimeter, area;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the radius of the circle:");
    circleRadius = input.nextFloat();

    perimeter = 2.0f * PI * circleRadius;
    area = PI * Math.pow( circleRadius, 2 );

    System.out.println("Perimeter: " + perimeter + "\n' + 
                       "Área: " + area);
  }

  static final float PI = 3.14159265f;
}
```

## Javascript implementation
```javascript
(function(){
  var circleRadius, perimeter, area;

  circleRadius = prompt('Type the radius of the circle:'); 
  circleRadius = parseFloat(circleRadius);

  perimeter = 2 * Math.PI * circleRadius;
  area      = Math.PI * Math.pow( circleRadius, 2 );

  console.log('Perimeter: ' + perimeter + '\n' + 
        'Area: ' + area);
}());
```
