# Java

OOPS
OOP stands for Object-Oriented Programming.
A class is a template for objects, and an object is an instance of a class.
Class is Fruit , Object -> Mango , Apple , Orange
A car is an object. The car has attributes, such as weight and color, and methods, such as drive and brake.


FINAL Keyword
If you don't want the ability to override existing values, declare the attribute as final:
The final keyword is useful when you want a variable to always store the same value, like PI (3.14159...).
The final keyword is called a "modifier


ABSTRACT
An abstract method belongs to an abstract class, and it does not have a body. The body is provided by the subclass
Abstraction lets you focus on what the object does instead of how it does it.
Abstraction is a process of hiding the implementation details and showing only functionality to the user.
The abstract keyword is a non-access modifier, used for classes and methods:
Abstract class: is a restricted class that cannot be used to create objects (to access it, it must be inherited from another class).
Abstract method: can only be used in an abstract class, and it does not have a body. The body is provided by the subclass (inherited from).
*Abstraction dont have body /
 * abstract body is provided by subclass 
abstarct class obj = new Subclass ();
Shape obj = new Circle1();


STATIC /PUBLIC
we created a static method, which means that it can be accessed without creating an object of the class, 
unlike public, which can only be accessed by objects


MULTIPLE CLASSES
Have created 2 classes First/Second , In First class methods declare & in Second have called those methods with
help of creating objects of main class .


CONSTRUCTOR
A constructor in Java is a special method that is used to initialize objects. 
The constructor is called when an object of a class is created. It can be used to set initial values for object attributes:
The constructor name must match the class name, and it cannot have a return type (like void)
All classes have constructors by default: if you do not create a class constructor yourself, Java creates one for you. However, then you are not able to set initial values for object attributes.


MODIFIERS
1)Acess Modifiers -> public , private , protected, default
public- >The code is accessible for all classes	
private	-> The code is only accessible within the declared class	
default	-> The code is only accessible in the same package. This is used when you don't specify a modifier. 	
protected -> The code is accessible in the same package and subclasses. 
2)Non - access Modifiers ->final , abstract
final	The class cannot be inherited by other classes.	
abstract	The class cannot be used to create objects (To access an abstract class, it must be inherited from another class. 


ENCAPSULATION
1)Encapsulation, is to make sure that "sensitive" data is hidden from users. 
declare class variables/attributes as private
2)provide public get and set methods to access and update the value of a private variable.
3)Private variables can only be accessed within the same class (an outside class has no access to it). However, it is possible to access them if we provide public get and set methods.
The get method returns the variable value, and the set method sets the value.
Class attributes can be made read-only (if you only use the get method), or write-only (if you only use the set method)
Flexible: the programmer can change one part of the code without affecting other parts
Increased security of data


PACKAGES
Packages are divided into two categories:
Built-in Packages (packages from the Java API)
User-defined Packages (create your own packages)
To create a package, use the package keyword:

import java.util.*;


INHERITANCE
Inheritance lets us inherit attributes and methods from another class
it is possible to inherit attributes and methods from one class to another. We group the "inheritance concept" into two categories:
subclass (child) - the class that inherits from another class
superclass (parent) - the class being inherited from
To inherit from a class, use the extends keyword.


POLYMORPHISM
Polymorphism means "many forms", and it occurs when we have many classes that are related to each other by inheritance.
Inheritance lets us inherit attributes and methods from another class. Polymorphism uses those methods to perform different tasks. This allows us to perform a single action in different ways.

For example, think of a superclass called Animal that has a method called animalSound(). Subclasses of Animals could be Pigs, Cats, Dogs, Birds - And they also have their own implementation of an animal sound (the pig oinks, and the cat meows, etc.):


INTERFACE
To access the interface methods, the interface must be "implemented" (kinda like inherited) by another class with the implements keyword (instead of extends).
ike abstract classes, interfaces cannot be used to create objects 
Interface methods do not have a body - the body is provided by the "implement" class
On implementation of an interface, you must override all of its methods
Interface methods are by default abstract and public
Interface attributes are by default public, static and final
An interface cannot contain a constructor (as it cannot be used to create objects)
Why And When To Use Interfaces?
1) To achieve security - hide certain details and only show the important details of an object (interface).
2) Java does not support "multiple inheritance" (a class can only inherit from one superclass). However, it can be achieved with interfaces, because the class can implement multiple interfaces. Note: To implement multiple interfaces, separate them with a comma (see example below).
//Interface is same as Inhertance , instead of extends use implements
 //create object of Subclass n called in main 

ENUM
An enum is a special "class" that represents a group of constants (unchangeable variables, like final variables).
Difference between Enums and Classes
An enum can, just like a class, have attributes and methods. The only difference is that enum constants are public, static and final (unchangeable - cannot be overridden).
An enum cannot be used to create objects, and it cannot extend other classes (but it can implement interfaces).
Why And When To Use Enums?
Use enums when you have values that you know aren't going to change, like month days, days, colors, deck of cards, etc.


SCANNER
The Scanner class is used to get user input, and it is found in the java.util package.
nextInt()	Reads a int value from the user
nextLine()	Reads a String value from the user


JAVA ARRAYLIST
The ArrayList class is a resizable array, which can be found in the java.util package.

The difference between a built-in array and an ArrayList in Java, is that the size of an array cannot be modified (if you want to add or remove elements to/from an array, you have to create a new one). While elements can be added and removed from an ArrayList whenever you want.
LOOP --->Loop through the elements of an ArrayList with a for loop, and use the size() method to specify how many times 
the loop should run.
Another useful class in the java.util package is the Collections class, which include the sort() method for sorting lists alphabetically or numerically:In the ArrayList chapter, you learned that Arrays store items as an ordered collection.



LINKED LIST
The LinkedList class is a collection which can contain many objects of the same type, just like the ArrayList.

The LinkedList class has all of the same methods as the ArrayList class because they both implement the List interface. This means that you can add items, change items, remove items and clear the list in the same way.The LinkedList stores its items in "containers." The list has a link to the first container and each container has a link to the next container in the list. To add an element to the list, the element is placed into a new container and that container is linked to one of the other containers in the list.
Use an ArrayList for storing and accessing data, and LinkedList to manipulate data.


JAVA HASHMAP
A HashMap however, store items in "key/value" pairs, and you can access them by an index of another type (e.g. a String).
One object is used as a key (index) to another object (value). It can store different types: String keys and Integer values, or the same type, like: String keys and String values:


HASHSET
A HashSet is a collection of items where every item is unique, and it is found in the java.util package:

ITERATOR
An Iterator is an object that can be used to loop through collections, like ArrayList and HashSet. It is called an "iterator" because "iterating" is the technical term for looping.
To use an Iterator, you must import it from the java.util package.

WRAPPER CLASS
Wrapper classes provide a way to use primitive data types (int, boolean, etc..) as objects.
Sometimes you must use wrapper classes, for example when working with Collection objects, such as ArrayList, where primitive types cannot be used (the list can only store objects):
ArrayList<int> myNumbers = new ArrayList<int>(); // Invalid
ArrayList<Integer> myNumbers = new ArrayList<Integer>(); // Valid
