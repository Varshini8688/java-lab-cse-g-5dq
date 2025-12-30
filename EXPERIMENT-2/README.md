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
## 2b) Title: Implement method overloading
## Source Code
``` java
 public class Sum{
     int Sum(int a,int b){
       return a+b;
     }
     int Sum(int a,int b,int c){
       return a+b+c;
     }
     double Sum(double a,double b){
       return a+b;
     }
   }
 class Main{
    public static void main(String[] args){
      Sum S = new Sum();
      System.out.println("Sum of the 2 integer: " +S.Sum(36,46));
      System.out.println("Sum of the 3 integers: " +S.Sum(20,36,46));
      System.out.println("SUm of the two real numbers: " +S.Sum(30.465,15.675));
    }
  }
```
## Output:
![Experiment-2b Output](sum.png)
## 2c) Title: Implement Constructor
## Source Code:
``` java
 class Student{
    String sname;
    int sage;
    double smarks;
  Student(String name,int age,double marks){
    sname = name;
    sage = age;
    smarks = marks;
  }
  void display(){
    System.out.println("Student name: " +sname);
    System.out.println("Student age: " +sage);
    System.out.println("Student marks: " +smarks);
  }
}
  class Main{
    public static void main(String[] args){
      Student s = new Student("varshini",18,965);
      s.display();
    }
  }
```
## Output:
![Experiment-2c Output](student.png)


