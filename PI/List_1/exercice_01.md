# Exercice 1

Find previous and next number of a given number.

Input: 
```
{Integer} number
```

Output: 
```
{Integer} previousNumber
{Integer} nextNumber
```

## Java implementation
```java
import java.util.Scanner;
public class Exercice01 {
  public static void main(String[] args){
    int prev, num, next;

    Scanner input = new Scanner(System.in);
    System.out.println("Type an integer:");
    num = input.nextInt();

    prev = num - 1;
    next = num + 1;

    System.out.println("Previous: " + prev);
    System.out.println("Next: " + next);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var prev, num, next;

  num = prompt('Type an integer:') | 0; 

  prev = num - 1;
  next = num + 1;

  console.log('Previous: ' + prev + '\n' + 
        'Next: ' + next);
}());
```
