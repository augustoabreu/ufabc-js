# Exercice 3

Calculate loan debt after 6 months late with rate of 5%.

Input: 
```
{Float} loanAmount
```

Output: 
```
{Float} debt
```

## Java implementation
```java
import java.util.Scanner;
public class Exercice03 {
  public static void main(String[] args){
    float loanAmount, debt;

    Scanner input = new Scanner(System.in);

    System.out.println("Type the loan amount:");
    loanAmount = input.nextFloat();

    debt = ( loanAmount * 5.0f / 100 ) * 6.0f + loanAmount;

    System.out.println("Debt: " + debt);
  }
}
```

## Javascript implementation
```javascript
(function(){
  var loanAmount, debt;

  loanAmount = prompt('Type the loan amount:'); 
  loanAmount = parseFloat(loanAmount);

  debt = ( loanAmount * 5 / 100 ) * 6 + loanAmount;

  console.log('Debt: ' + debt);
}());
```
