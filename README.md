# Fundamentals-OOP-java
Pluralsight Course



Something you already know:
(Pluralsight lesson)

  Objects:
    - State( data)
    - Behavior ( method and functions)
  
   - Encapsulation and abstraction  
   - Inheritance and polymorphism
   - Interfaces and system design


Advantages - same with Python
  
    OOP is faster and easier to execute
    OOP provides a clear structure for the programs
    OOP helps to keep the Java code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug
    OOP makes it possible to create full reusable applications with less code and shorter development time

General Ideas:
  
      Class:
          Instances - a class is a template for objects, and an object is an instance of a class.
          
      has-a: belonging
      is- a: description
      
  
Review Packages -- can be done in IntelliJ:
  
        1) go to src, right click to New;
        2) create class, name: com.pluralsight.NAME.Main
        3) copy original Main content into this one.
        
        why we need package? Java 中的包用于对相关类进行分组。将其视为文件目录中的文件夹。我们使用package来避免名称冲突，并编写更好的可维护代码。It's like creat a folder to wrap them. 
        ** use the backwards method:com. at the front
  
   Gernate
   
        Automatically change it into String.
        Right click in the comment line; choose Gernate; select toString; select the items you want.
        Then it automatically build a coding block.
        
        
 
Questions about the coding pieces.

Optional<> ?
HashMap?
Why we have catalogue?
Customer.java - change into another line

relations: catalogue ->productType; product; 
Terms :

      Encapsulation: 封装. combining the data members and data methods of the class inside the user-defined class.
      Assign Responsibilities: 分配责任 two class may use same object (customer + credit card - payment)
      High coupling: 高耦合. When two classes are highly dependent on each other. Not good, if you change one item, has to change another one!
      SRP: Single Responsibility Principle - A class should have only one reason to change
      DRY: Don't Repeat Youself
      Overriding: 重写覆盖.subclass change the parent/superclass. 只从下往上，不改变同级子类
      Polymorphism: 多态性. allows us to perform the same action in many different ways. Usually via overriding
      Inheritance: 继承. lets us inherit attributes and methods from another class.
      enum: enumerate. 枚举是一个特殊的“类”，表示一组常量（不可更改的变量，如最终变量）。
            主要区别在于 <array> 是一个值，而 <enum> 是一种类型。
      super(): quote the parent parameter from above level.
     
     E.g of Inheritance/ Overriding/ Polymorphism:
     
          class Animal {
            public void animalSound() {
              System.out.println("The animal makes a sound");
            }
          }           // superclass

          class Pig extends Animal {
            public void animalSound() {
              System.out.println("The pig says: wee wee"); // overriding the print content
            }
          }          // subclass 1: use 'extends' to inherit from the super class, so have the print

          class Dog extends Animal {
            public void animalSound() {
              System.out.println("The dog says: bow wow");
            }
          }         // subclass 2

          class Main {
            public static void main(String[] args) {
              Animal myAnimal = new Animal();
              Animal myPig = new Pig();
              Animal myDog = new Dog();

              myAnimal.animalSound();
              myPig.animalSound(); 
              myDog.animalSound();
            }
          }         // call the method


          Print:
          
          The animal makes a sound
          The pig says: wee wee     // overriding results. not"The animal..." but "The pig says..."  
          The dog says: bow wow     // demonstrating polymorphism

      
Logic & Design:

  Find out the objects, relationships within the events, and then establish the class/ functions accordingly.
  Demo, Catalogue & ProductType are the 3 extra ones. 


  why the lineitem have no "final" ? 



