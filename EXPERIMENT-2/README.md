# Experiment-2
## 2a) Title:Create a class,methods and invoke them inside main method
## Source Code
``` java
 public class Rectangle{
    double length;
    double breadth;
  double area(){
    return length*breadth;
  }
  double perimeter(){
    return 2*(length+breadth);
  }
 }

 class Main{
    public static void main(String[] args){
      Rectangle rect = new Rectangle();
      rect.length = 10;
      rect.breadth = 5;
      double area = rect.area();
      double perimeter = rect.perimeter();
      System.out.println("Area of a given rectangle: " +area);
      System.out.println("Perimeter of a given rectangle: " +perimeter);
    }
  }
```
## Output:
![Experiment-2a Output](rect.png)
