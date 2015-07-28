# Exercice 12

Calculate arithmetical progression from a ratio.

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
public class Ex12 {
  public static void main(String[] args){
    float ratio, ap = 0, firstTerm;
    int counter = 1;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the ratio of the arithmetical progression:");
    ratio = input.nextFloat();

    System.out.println("Type the first term of the arithmetical progression:");
    firstTerm = input.nextFloat();

    while (counter <= 20) {
        ap = ap + (firstTerm + (counter - 1) * ratio);
        counter += 1;
    }

    System.out.println("20th term: " + ap);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var ratio, ap = 0, firstTerm, counter = 1;

  ratio = prompt('Type the ratio of the arithmetical progression:'); 
  ratio = parseFloat(ratio);

  firstTerm = prompt('Type the first term of the arithmetical progression:'); 
  firstTerm = parseFloat(firstTerm);
  
  while (counter <= 20) {
    ap = ap + (firstTerm + (counter - 1) * ratio);
    counter += 1;
  }

  alert('20th term: ' + ap);
}());
```
