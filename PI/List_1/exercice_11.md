# Exercice 11

Verify if the inserted segments form a triangle.

Input: 
```
{Float} circX
{Float} circY
{Float} ptX
{Float} ptY
{Float} radius
{Float} hypotenuse
```

Output: 
```
{String} pointIsInsideOfCircle
```

## Java implementation
```java
import java.util.Scanner;
public class Ex11 {
  public static void main(String[] args){
    float circX, circY, ptX, ptY, radius, hypotenuse;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the X coordinate of the center of the circle:");
    circX = input.nextFloat();

    System.out.println("Type the Y coordinate of the center of the circle:");
    circY = input.nextFloat();

    System.out.println("Type the radius of the circle:");
    radius = input.nextFloat();

    System.out.println("Type the X coordinate of the point:");
    ptX = input.nextFloat();

    System.out.println("Type the Y coordinate of the point:");
    ptY = input.nextFloat();

    hypotenuse = Math.sqrt(Math.pow((ptX - circX), 2) + Math.pow((ptY - circY), 2));

    if (hypotenuse <= radius) {
      System.out.println("The point is inside of the circle");
    } else {
      System.out.println("The point is not inside of the circle");
    }
  }
}
```

## Javascript implementation
```javascript
(function(){
  var circX, circY, ptX, ptY, radius, hypotenuse;

  circX = prompt('Type the X coordinate of the center of the circle:'); 
  circX = parseFloat(circX);

  circY = prompt('Type the Y coordinate of the center of the circle:'); 
  circY = parseFloat(circY);

  radius = prompt('Type the radius of the circle:'); 
  radius = parseFloat(radius);

  ptX = prompt('Type the X coordinate of the point:'); 
  ptX = parseFloat(ptX);

  ptY = prompt('Type the Y coordinate of the point:'); 
  ptY = parseFloat(ptY);

  hypotenuse = Math.sqrt(Math.pow((ptX - circX), 2) + Math.pow((ptY - circY), 2));

  if (hypotenuse <= radius) {
    console.log('The point is inside of the circle');
  } else {
    console.log('The point is not inside of the circle');
  }
}());
```
