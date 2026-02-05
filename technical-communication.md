## Context 
You joined a new project. The project codebase is difficult to manage. Your team lead has asked to study a few concepts and refactor the codebase. Create a report on OOP with code samples

## What is OOP
* OOP means object oriented programming. It is a methodology where we can assume everything in life as an object.
* In OOP we have mainly Class, Object, Method and four pillars
* The four pillars are the main advantage in OOP.

## Why OOP
* It reuses the code
* Provides flexibility
* Provides security via encapsulation

## Pillars of OOP
### 1. Inheritance
* Inheritance means one class can use the properties and methods of another class.
* It helps in code reuse.
* Child class can extend parent class using extends keyword.
* Advantage - code reusability

```java
    class Animal {
        void eat() {
            System.out.println("This animal eats food.");
        }
    }
    
    class Dog extends Animal {
        void bark() {
            System.out.println("The dog barks.");
        }
    }
    
    public class TestInheritance {
        public static void main(String[] args) {
            Dog dog = new Dog();
            dog.eat(); 
            dog.bark(); 
        }
    }
```


### 2. Abstraction
* Abstraction means hiding implementation details and showing only required methods.
* It is achieved using interface or abstract class.
* User does not know how things work internally.

```java
    abstract class Shape {
        abstract void draw();
    }
    
    class Circle extends Shape {
        void draw() {
            System.out.println("Circle");
        }
    }
    
    class Main {
        public static void main(String[] args) {
            Shape s = new Circle();
            s.draw();
        }
    }
```

### 3. Encapsulation
* Encapsulation means binding data and methods together.
* Variables are kept private.
* Access is given using getters and setters.
* Advantages - data hiding, increases flexibility, improved maintainability

```java
    class Student {
        private String name;
    
        public void setName(String name) {
            this.name = name;
        }
    
        public String getName() {
            return name;
        }
    }
    
    class Main {
        public static void main(String[] args) {
            Student s = new Student();
            s.setName("John");
            System.out.println(s.getName());
        }
    }
```

### 4. Polymorphism 
* Polymorphism means one method, many forms.
* Same method behaves differently for different objects.
* Achieved using method overriding, method overloading and interfaces.

```java
    class MathOperation {
        int add(int a, int b) {
            return a + b;
        }
    
        int add(int a, int b, int c) {
            return a + b + c;
        }
    }
    
    public class TestOverloading {
        public static void main(String[] args) {
            MathOperation mathOp = new MathOperation();
            System.out.println(mathOp.add(5, 10)); 
            System.out.println(mathOp.add(5, 10, 15)); 
        }
    }
```


## Resources 
[Resource 1 - CodeSignal](https://codesignal.com/learn/courses/refactoring-code-for-readability-and-maintainability-2/lessons/object-oriented-programming-oop-principles-and-code-refactoring-in-java?utm_source=chatgpt.com)<br>
[Resource 2 - Medium](https://medium.com/javajams/java-refactoring-transforming-messy-code-into-elegant-solutions-386263e7d044)<br>
[Resource 3 - Geeks For Geeks](https://www.geeksforgeeks.org/java/object-oriented-programming-oops-concept-in-java/)<br>
[Resource 4 - Medium](https://medium.com/@suraif16/object-oriented-programming-9e4627abf1be)
