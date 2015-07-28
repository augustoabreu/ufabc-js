# Exercice 9

Verify if the inserted segments form a triangle.

Input: 
```
{Float} segment1
{Float} segment2
{Float} segment3
```

Output: 
```
{String} formTriangleOrNot
```

## Java implementation
```java
import java.util.Scanner;
public class Ex9 {
  public static void main(String[] args){
    float segment1, segment2, segment3;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the first segment size:");
    segment1 = input.nextFloat();

    System.out.println("Type the second segment size:");
    segment2 = input.nextFloat();

    System.out.println("Type the third segment size:");
    segment3 = input.nextFloat();

    if (segment1 < ( segment2 + segment3 ) && 
        segment2 < ( segment1 + segment3 ) && 
        segment3 < ( segment1 + segment2 )) {
        System.out.println("The segments form a triangle.");
    } else {
        System.out.println("The segments do not form a triangle.");
    }
  }
}
```

## Javascript implementation
```javascript
(function(){
  var segment1, segment2, segment3;

  segment1 = prompt('Type the first segment size:'); 
  segment1 = parseFloat(segment1);

  segment2 = prompt('Type the second segment size:'); 
  segment2 = parseFloat(segment2);

  segment3 = prompt('Type the third segment size:'); 
  segment3 = parseFloat(segment3);

  if (segment1 < ( segment2 + segment3 ) && 
      segment2 < ( segment1 + segment3 ) && 
      segment3 < ( segment1 + segment2 )) {
      console.log('The segments form a triangle.')
    } else {
      console.log('The segments do not form a triangle.')
    }
}());
```
