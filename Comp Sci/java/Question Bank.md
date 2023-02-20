
#### 1. Explain the different types of constructors in java Define static filed and method? Explain with an example.
==> In Java, a constructor is a special type of method that is used to initialize an object of a class. There are two main types of constructors in Java:
1.  Default Constructor: This constructor has no parameters and is automatically created by the compiler if no other constructors are defined in the class. The purpose of the default constructor is to provide a default initial state for the object.
2.  Parameterized Constructor: This constructor takes one or more parameters and is used to initialize the object with specific values.
Here is an example to demonstrate the use of default and parameterized constructors in Java:

```java
public class Student {
  int id;
  String name;

  // Default Constructor
  Student() {
	System.out.println("Default Constructor is called");
  }

  // Parameterized Constructor
  Student(int id, String name) {
    this.id = id;
    this.name = name;
  }

  public static void main(String[] args) {
    // Default Constructor
    Student s1 = new Student();

    // Parameterized Constructor
    Student s2 = new Student(123, "John");
  }
}
```

In this example, we have defined a class `Student` with two instance variables, `id` and `name`. The class has two constructors, a default constructor and a parameterized constructor. The default constructor has no parameters and simply prints a message to the console. The parameterized constructor takes two parameters, `id` and `name`, and sets the values of the corresponding instance variables.

Static fields and methods are members of a class that belong to the class itself, rather than to an instance of the class. They can be accessed without creating an object of the class.

Here is an example to demonstrate the use of a static field and method in Java:

```java
public class MathUtils {
  // Static field
  public static final double PI = 3.14;

  // Static method
  public static double calculateCircleArea(double radius) {
    return PI * radius * radius;
  }

  public static void main(String[] args) {
    double area = MathUtils.calculateCircleArea(10);
    System.out.println("Area of the circle: " + area);
  }
}
```

In this example, we have defined a class `MathUtils` with a static field `PI` and a static method `calculateCircleArea`. The `PI` field is a constant with the value `3.14`, and the `calculateCircleArea` method calculates the area of a circle given its radius. The method uses the `PI` field as the value of π. The `main` method calls the `calculateCircleArea` method without creating an object of the `MathUtils` class, as it is a static method.


#### 2. Explain any four features of java programming.
==> 
1.  Object-Oriented Programming: Java is an object-oriented programming language, which means it is based on the concept of objects and classes. Objects represent real-world entities, and classes define the properties and behaviors of these objects.
2.  Platform Independent: Java is a platform-independent language, which means that the same code can be run on any device or operating system without modification. This is achieved through the use of the Java Virtual Machine (JVM), which acts as an intermediary between the code and the underlying hardware.
3.  Memory Management: Java provides automatic memory management through the use of a garbage collector. The garbage collector frees up memory occupied by objects that are no longer being used, freeing the developer from the responsibility of manually managing memory.
4.  Multithreaded: Java supports multithreading, which allows multiple threads of execution to run concurrently within a single program. This enables the creation of highly concurrent and responsive applications, and is particularly useful for applications that require multiple tasks to run in parallel.

#### 3. Write a java program to display all the odd numbers between 1 to 30 using for loop & if
==> Here is a program to display all the odd numbers between 1 and 30 using for loops & if

```java
public class oddNums {
	public static void main(String[] args) {
		System.out.println("following are the ")
		for(int i = 1; i <= 30; i++) {
			if (i % 2 != 0)
				System.out.println(i);
		}
	}
}
```


#### 4. Discuss the various characteristics of object oriented programming concepts?
==> Object-oriented programming (OOP) is a programming paradigm that is based on the concept of objects and classes. The following are the main characteristics of OOP:
1.  Encapsulation: Encapsulation is the mechanism of hiding the implementation details of a class from its clients. This means that the internal workings of a class are hidden from the outside world, and clients can interact with the class only through its public methods and properties. This helps to maintain the integrity of the data within the object and reduces the risk of unintended changes.
2.  Abstraction: Abstraction is the process of abstracting away the implementation details of a class and exposing only the essential characteristics and behaviors of the class. This makes it easier to reason about the class, and reduces the complexity of the code.
3.  Inheritance: Inheritance is the mechanism by which a new class can be derived from an existing class. The derived class inherits all of the properties and behaviors of the base class, and can also add new properties and behaviors of its own. This enables code reuse and reduces the amount of redundant code in a system.
4.  Polymorphism: Polymorphism is the ability of an object to take on multiple forms. This allows objects of different classes to be treated as objects of a common base class, and enables the implementation of generic algorithms that can work with objects of different types.
5.  Composition: Composition is the mechanism by which objects can be composed of multiple other objects, allowing for the creation of complex objects from simpler building blocks. This enables the creation of highly modular systems that can be easily maintained and modified.
These characteristics of OOP make it a powerful programming paradigm for developing complex software systems, and are widely used in many programming languages, including Java, C++, and Python.

#### 5. Write a Java program to check if the given number is a prime number.
==> Following is the code for,
```java
public primes {
	public boolean isPrime(int num) {
		for (int i = 2; i < num / 2; i++) {
			if (num % i == 0)
				return false;
		}
		return true;
	}

	public static void main(String[] args) {
		int number = 11;
		if (isPrime(number))
			System.out.println(number + " is a prime number");
		else
			System.out.println(number + " is not a prime number");
	}
}
```
