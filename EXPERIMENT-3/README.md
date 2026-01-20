# Experiment-3a
## 3a) Title: Implement Constructor Overloading In Java.
## Source Code
```
class Student { 
    String name; 
    int age; 
    double marks; 
    Student() {
    }
    Student(String name, int age, double marks){
        this.name=name;
        this.age=age;
        this.marks=marks;
    }
    void display(){
        System.out.println("Name="+name);
        System.out.println("Age="+age);
        System.out.println("marks="+marks);
    }
}
class Main{ 
    public static void main(String args[]){
        Student std=new Student();
        std.display();
        Student std1=new Student("Varshini",19,95.5);
        std1.display();
    }
}
```
## Output
![exp-3a output](student.png)

# Experiment 3b
## 3b) Title: Binary Search.
## Source Code:
```
import java.util.Scanner;
class BinarySearch {
    int[] list;
    int size;
    BinarySearch(int size) {
        this.size=size;
        list = new int[size];
    }
    void setList() {
        Scanner sc = new Scanner(System.in);
        for (int i=0; i < size; i++) {
            System.out.print("Enter item "+(i+1) + ".");
            list[i] = sc.nextInt();
        }
    }
    void getList() {
         for (int i=0; i < size; i++) {
             if (i==size-1)
                System.out.print(list[i]+".");
             else
                System.out.print(list[i]+",");
             }
             System.out.println();
    }
    int binarySearch(int key) {
        int low=0, high = size-1;
        while(low<=high) {
        int mid= (low+high)/2;
        if(list[mid]==key)
          return mid;
        else if(list[mid] < key)
             low = mid+1;
        else
             high = mid-1;
        }
        return -1;
    }
}
import java.util.Scanner;
class Main {
      public static void main(String[] args) {
      Scanner sc = new Scanner(System.in);
      System.out.print("Enter size: ");
      int size = sc.nextInt();
      BinarySearch bs= new BinarySearch(size);
      bs.setList();
      System.out.print("list elements:");
      bs.getList();
      System.out.print("Enter key:");
      int key = sc.nextInt();
      int index = bs.binarySearch(key);
      if (index == -1)
          System.out.println("Element not found");
      else
          System.out.println("Element found at index: " + index);
    }
}

```
## Output:
![exp-3b output](binary.png)
# Experiment 3c
## 3c) Title: Bubble sort.
## Source Code:
```
class Bubblesort { 
      void Bubblesort(int arr[]) { 
      int n = arr.length; 
      int temp=0; 
      for(int i=0; i<n-1; i++) {
       for(int j=0; j<n-i-1; j++) {
             if(arr[j]>arr[j+1]) {
                 temp=arr[j+1];
                 arr[j+1]=arr[j];
                 arr[j]=temp;
             }
            }
           }
          }
         }

import java.util.Scanner;
class main {
     public static void main(String[] args) {
           System.out.println("Enter the size of the array:");
           Scanner sc= new Scanner(System.in);
           int size= sc.nextInt();
           int integer[] = new int[size];
              for(int i = 0; i < size; i++) {
           System.out.print("Enter the value of integer at index " + (i+1) + ":");
                  integer[i] = sc.nextInt();
           }
            Bubblesort bs = new Bubblesort ();
            bs.Bubblesort(integer);
            System.out.println("The sorted integers: ");
            for(int i=0; i<size; i++){
                  if(i==size-1)
                System.out.print(integer[i]  +  ".");
                  else
                System.out.print(integer[i] + ",");
          }
      }
    }
```
## Output
![exp-3c output](bubblesort.png)










