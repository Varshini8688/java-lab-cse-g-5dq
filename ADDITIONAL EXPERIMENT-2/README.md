# ADDEXP-2
## Title: sum of the frist n Fibonacci Numbers
## Source Code:
``` java
 class Fibonacci{
    int n,a=0,b=1,c,sum=0;
    Fibonacci(int n){
      this.n = n;
    }
    void printFib(){
      for(int i=1;i<=n;i++){
        if(i==1)
          c = a;
        else if(i==2)
          c = b;
        else{
          c = a+b;
          a = b;
          b = c;
        }
        sum+=c;
        if(i==n)
          System.out.print(c + ".");
        else
          System.out.print(c + ", ");
      }
    }
    int getsum(){
      return sum;
    }
  }
 import java.util.Scanner;
 class Main{
    public static void main(String[] args){
      Scanner sc = new Scanner(System.in);
      System.out.print("enter no of terms: ");
      int n = sc.nextInt();
      if(n>0){
      Fibonacci f = new Fibonacci(n);
      System.out.print("Fib series are:");
      f.printFib();
      System.out.println("\nsum = " + f.getsum());
      }
      else{
           System.out.println("Fibonacci sequence canot be calculated");
      }
   }

 }
```
## Output:
![ADDEXP-2 Output](fib.png)
