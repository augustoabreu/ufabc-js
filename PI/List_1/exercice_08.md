# Exercice 8

Calculate hypotenuse of a triangle.

Input: 
```
{Float} cateto1
{Float} cateto2
```

Output: 
```
{Float} hypotenuse
```

## Java implementation
```java
import java.util.Scanner;
public class Ex8 {
  public static void main(String[] args){
    float cateto1, cateto2, hypo;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the size of the first cateto:");
    cateto1 = input.nextFloat();

    System.out.println("Type the size of the second cateto:");
    cateto2 = input.nextFloat();

    hypo = Math.sqrt( Math.pow( cateto1, 2 ) + Math.pow( cateto2, 2 ) );
    System.out.println("Hypotenuse: " + hypo );
  }
}
```

## Javascript implementation
```javascript
(function(){
  var cateto1, cateto2, hypo;

  cateto1 = prompt('Type the size of the first cateto:'); 
  cateto1 = parseFloat(cateto1);

  cateto2 = prompt('Type the size of the second cateto:'); 
  cateto2 = parseFloat(cateto2);
  
  hypo = Math.sqrt( Math.pow( cateto1, 2 ) + Math.pow( cateto2, 2 ) );

  alert('Hypotenuse: ' + perimeter);
}());
```
