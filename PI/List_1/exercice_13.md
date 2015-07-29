# Exercice 13

Calculate geometric progression from a ratio.

Input: 
```
{Float} ratio
{Float} firstTerm
```

Output: 
```
{Float} 20th_term
```

## Java implementation
```java
import java.util.Scanner;
public class Ex13 {
  public static void main(String[] args) {
    float firstTerm, ratio, gp, pow;

    Scanner input = new Scanner( System.in );

    System.out.println("Type the first term of the geometric progression:");
    firstTerm = input.nextFloat();

    System.out.println("Type the ratio of the geometric progression:");
    ratio = input.nextFloat();

    pow = Math.pow(ratio, 20);
    gp = firstTerm * pow;

    System.out.println("20th term: " + gp);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var ratio, gp = 0, firstTerm, pow;

  ratio = prompt('Type the ratio of the geometric progression:'); 
  ratio = parseFloat(ratio);

  firstTerm = prompt('Type the first term of the gemetric progression:'); 
  firstTerm = parseFloat(firstTerm);
  
  pow = Math.pow(ratio, 20);
  gp = firstTerm * pow;

  console.log('20th term: ' + gp);
}());
```
