# Errata for *Java. The Comprehensive Guide*

This repository collects and tracks errors, corrections, and clarifications for my book *Java. The Comprehensive Guide*.

## 📚 Book Details  
- **Title:** *Java. The Comprehensive Guide*  
- **Author:** Christian Ullenboom  
- **Publisher:** Rheinwerk Computing  
- **ISBN:** 978-1493222957  

## 📖 About this page
Despite my best efforts, the occasional typo, logic mishap, or rogue semicolon have snuck into my book. This repository serves as a centralized place to report and document any inaccuracies, typos, or clarifications.

## 📌 How to Report an Issue  

Spotted an error? Here’s how you can help:

- Specify the **chapter**, **paragraph**, or **code listing** where the issue appears.
- Provide a clear **description** of the problem.
- If possible, suggest a **correction or clarification**.

Your feedback is greatly appreciated—thank you for helping improve the book.

## 📝 Errata List  

### Chapter 1: Introduction  

#### The Development of Java and Its Future Prospects

- ❌ Twenty years ago, Java had two major advantages: simplicity compared to its predecessor C++ and the absence of “dangerous” syntactic constructs.
- ✅ **About 25** years ago, Java had two major advantages: simplicity compared to its predecessor C++ and the absence of “dangerous” syntactic constructs.

#### A Square Numbers Program

- ❌ A Square Numbers Program
- ✅ **Bottles of Beer: The Countdown Continues!**

#### The Compiler Run

- ❌ Now, let’s change to the command prompt **console** and navigate to the directory with the source code. If 
- ✅ Now, let’s change to the command prompt and navigate to the directory with the source code. If 


### Chapter 2:	Imperative Language Concepts

#### Relational Operators and Equality Operators

- ❌ Greater than or equal to (≥)
- ✅ Greater than or equal to (>=)

- ❌ Less than or equal to (≤)
- ✅ Less than or equal to (<=)

#### Overloaded Plus for Strings*

- ❌ If the expression around the condition operator were not parenthesized, then the plus operator would append the 1 to the string, and the > operator would occur. That operator, however, expects compatible data types, which aren’t given in our case as the string would be on the left and the integer 2 on the right. 
- ✅ If the expression around the condition operator were not parenthesized, then the plus operator would append the **content of quantity** to the string **"You have "**, and the **==** operator would occur. That operator, however, expects compatible data types, which aren’t given in our case as the string would be on the left and the integer **12** on the right.

#### print(…) und println(…) Are Overloaded

- ❌ If now the print(...) method is called with any object type, then the best fitting method is selected. This selection process works even for arbitrary objects, as described in Chapter 7, Section 7.5.2.

- ✅ If now the print(...) method is called with **an argument of any type, the best-fitting method is selected**. This selection process applies even to arbitrary objects, as explained in Chapter 7, Section 7.5.2.


###	Chapter 3: Classes and Objects

(none)


###	Chapter 4: Arrays and Their Areas of Uses

#### Arrays Are Pretty Normal Objects

- ❌ An array object has an object variable named length, and methods are declared on the array object, such as clone() and everything that java.**long**.Object has.
- ✅An array object has an object variable named length, and methods are declared on the array object, such as clone() and everything that java.**lang**.Object has. 

#### Arrays with { contents }

- ❌ `"Caramellos," "Gummi Fish."`
- ✅ `"Caramellos", "Gummi Fish",`

- ❌ `double[] prices = new int[0]`
- ✅ `double[] prices = new double[0];`

#### Array Lengths Are Final

- ❌ The **object variable attribute** length of an array isn’t only public and of type int, but of course also final
- ✅ The **instance variable** length of an array isn’t only public and of type int, but of course also final


### Chapter 5: Handling Characters and Strings

#### 5.1.5 Escape Sequences

- ❌ double**qou**te
- ✅ double**Quo**te

- ❌ This text block becomes the string "1\u0002". 
- ✅ This text block becomes the string **"1\n2"**.

#### 5.3.1 Is That So?

- ❌ The term “letter” not only describes well-known letters like “a” or “α.” Unicode contains more about than 100,000 characters, including hundreds of letters.
- ✅ The term “letter” not only describes well-known letters like “a” or “α.” Unicode contains more about than **150,000** characters, including hundreds of letters **from different languages**.

#### 5.4 Strings

- ❌ A string is a collection of characters **(data type char)** that the runtime environment stores in the memory in an orderly fashion
- ✅ A string is a collection of characters that the runtime environment stores in the memory in an orderly fashion

#### 5.5.9 Extracting String Sections > Other Options for Decomposition

- ❌ “
- ✅ "

#### 5.5.12 Creating String Objects with Constructors and from Repeats

- ❌ `isAnangram`
- ✅ `isAnagram`

#### 5.7.3 Default Methods in the CharSequence Interface

- ❌ This interface has two default methods:
- ✅ This interface has **three** default methods:

#### 5.11.1 Formatting and Outputting via format() > Pimp My String with Format Specifiers

- ❌ If format(...) or printf(...) is called without a locale, the default language of the operating system is used.
- ✅ If format(...) or printf(...) is called without a locale, the default language of the operating system is used **(assume it is English)**.

- ❌ System.out.printf( Locale.ENGLISH, "%.2f%n", bitcoinPrice );
- ✅ System.out.printf( Locale.**GERMAN**, "%.2f%n", bitcoinPrice );

- ❌ 46714,42 \n   46714.42
- ✅ 46714.42 \n   46714,42    


### Chapter 6: Writing Custom Classes

#### enum constants in switch

- ❌ Enum constants can be used in switch statements. Let’s initialize a variable of type CandyType and use a case distinction with the enumeration for a test on two candy types; we’ll use three alternative notations
- ✅ Enum constants can be used in switch statements **and switch expressions**. Let’s initialize a variable of type CandyType and use a **switch-case** with the enumeration for a test on two candy types; we’ll use three alternative notations

- ❌ “
- ✅ "

#### Initializing Object Variables

- ❌ Then, the compiler automatically generates some additional **lines** because—to put it simply—no code is allowed outside constructors and methods
- ✅ Then, the compiler automatically generates some additional **statements** because—to put it simply—no code is allowed outside constructors and methods


### Chapter 7:	Object-Oriented Relationship

#### Is-a-Type-of Relationships and Automatic Typecasting

- ❌ •	An event is an `Event`.
- ✅•	An `Event` is an `Event`.

#### No Arbitrary Type Tests with instanceof

- ❌ The expression is incorrect because StringBuilder is not a base class for String.
- ✅ The expression is incorrect because **Event** is not a base class for String.


### Chapter 8: Interfaces, Enumerations, Sealed Classes, Records

#### Code Compatibility and Binary Compatibility

- ❌ For example, if the interface is modified, recompiled, and placed in the module path, the following tasks are fine
- ✅ For example, if the interface is modified, recompiled, and placed in the **class** path, the following **changes** are fine

#### 8.4.2 Records with Methods

- ❌ return new Point2D.Double( longitude, latitude );
- ✅ return new Point2D.Double( latitude, longitude );

- ❌ 2 x return new Location( longitude, latitude )
- ✅ 2 x return new Location( latitude, longitude )

- ❌ System.out.println( "Access" + longitude );
- ✅ System.out.println( "Access " + longitude );


### Chapter 9: There Must Be Exceptions

#### Exceptions in Java with try and catch

- ❌ The `try block` is usually  followed by a catch block ... 
- ✅ The `try` is usually  followed by a catch block ... 

- ❌ Program code that can execute an exception
- ✅ Program code that can **raise** an exception

#### Types That Are AutoCloseable and Closeable

- ❌ and Closable with every resource 
- ✅ and Clos**e**able with every resource 

#### 9.9.3 Enabling or Disabling Assertions More Detailed

- ❌ [eg] Example Box
- ✅ [eg] Example
```Assertions can be enabled or disabled selectively for classes, packages, or system classes. The switches -ea (enable assertions), -da (disable assertions), and -esa (enable system assertions, for classes such as those in java.lang) provide fine-grained control. A few examples:
Enable assertions only for class com.tutego.App:
$ java -ea:com.tutego.App ClassWithMain
Enable assertions for all classes (including the default package):
$ java -ea ClassWithMain
Enable assertions for package com.tutego and all its subpackages (...):
$ java -ea:com.tutego... ClassWithMain
Enable assertions for com.tutego and its subpackages, but disable them for class com.tutego.App:
$ java -ea:com.tutego... -da:com.tutego.App ClassWithMain
```


### Chapter 10: Nested Types

#### 10.2 Static Nested Types

- ❌ Listing 10.1:: src/main/java/com/tutego/insel/nested/Lamp.java
- ✅ Listing 10.1:: src/main/java/com/tutego/insel/nested/**SquirrelNutCaramel**.java

#### 10.3 Non-Static Nested Types

- ❌ Let’s declare an inner class named Room in House with the following example code:
- ✅ Let’s declare an inner class named **Coconut** in **AlmondJoy** with the following example code:

#### 10.3.1 Creating Instances of Inner Classes

- ❌ To create an object in the static main(String[]) method of the house, you can write the following code:
- ✅ To create an object **of type Coconut** in the static main(String[]) method of the **class AlmondJoy**, you can write the following code:

#### 10.5.3 Constructors of Anonymous Inner Classes

- ❌ new java.math.BigDecimal( "12345678901234567890" )
- ✅ new java.math.Big**Integer**( "12345678901234567890" )

#### 10.6 Nests

- ❌ new In1().intern**1**w();
- ✅ new In1().internw();


### Chapter 11: Special Types of Java SE

#### 11.4.1 Naturally Ordered or Not?

- ❌ String**, StringBuilder, and StringBuffer**
- ✅ String

#### 11.4.6 Static and Default Methods in Comparator > Sequence of Comparators

- ❌ Let’s now use these thenComparing(...) methods from Comparator in an example that sorts a list of names last name and then by first name.
- ✅ Let’s now use these thenComparing(...) methods from Comparator in an example that sorts a list of **calories and name**.

- ❌ Basically, this method is a Comparator with a compare(Comparable**<Object>** c1, Comparable**<Object>** c2) method that returns c2.compareTo(c1).
- ✅ Basically, this method is a Comparator with a compare(Comparable c1, Comparable c2) method that returns c2.compareTo(c1).

#### 11.5.8. Handling Unsigned Numbers*

- ❌ to the range of –127 to 128
- ✅ to the range of –12**8** to 12**7**

- ❌ toUnsignedString(…) and parseUnsignedString(…)
- ✅ toUnsignedString(…) and parseUnsigned**[Int|Long]**(…)


### Chapter 12: Generics<T>

#### 12.1.7 Generic Methods/Constructors and Type Inference > Quite by Chance One or the Other Argument

- ❌ In the following example, T in sit(...) doesn’t refer to the parameter variable of the Lupilu class, but does refer to the parameter value of the method:
- ✅ In the following example, T in sit(...) doesn’t refer to the parameter variable of the Lupilu **interface**, but does refer to the parameter value of the method:

#### 12.2.2 Type Erasure

- ❌ return vale;
- ✅ return val**u**e;

#### 12.5.2 Generics Aren’t Covariant, but Invariant

- ❌ Then, p.set(2.2) isn’t OK, for example, because Double isn’t compatible with Integer.
- ✅ Then, **r**.set(2.2) isn’t OK, for example, because Double isn’t compatible with Integer.

#### 12.5.4 Bounded Wildcards

- ❌ All possible Number objects can be in the rocket p.
- ✅ All possible Number objects can be in the rocket **r**.

#### 12.6.1 Type Tokens

- ❌ `Class<String> clazz = "Simulatte.getClass();`
- ✅ `Class<String> clazz = "Simulatte".getClass();`


### Chapter 13: Lambda Expressions and Functional Programming

#### Parameter Types

- ❌ class OverloadedFuntionalInterfaceMethods
- ✅ class OverloadedFun**c**tionalInterfaceMethods

#### Short Version 2: The Lambda Body Is Either a Single Expression or a Block

- ❌ If you used an explicit return in line (1), everything would be fine; if you omitted the return in line (2), the line would also be compilable.
- ✅ If in (1) we used an explicit return and ended the expression with a semicolon, , everything would be fine; if you omitted the return in line (2), the line would also be compilable.

#### Writing Constructor References

- ❌ .map( BigDecimal::valueOf ) 
- ✅ .map( value -> new BigDecimal( value ) )

- ❌ .map( BigDecimal::valueOf )
- ✅ .map( BigDecimal::new )

#### I Take Two

- ❌ BiConsumer, BiFunction and BiPredicate in the first column
- ✅ has to be in the second colum

#### 	Starting Functional Interfaces with Optional

- ❌ final class java.lang.Optional<T>  
- ✅ final class java.**util**.Optional<T> 


### Chapter 14: Architecture, Design, and Applied Object Orientation

(none)


### Chapter 15: Java Platform Module System

#### Module Migration

- ❌ required guava
- ✅ require**s** guava

#### 15.3.10 Module Migration

- ❌ **Guava doesn’t set a module name.**
- ✅ Guava uses (and since version 33.4.8, it even ships as a proper module under that name): `Automatic-Module-Name: com.google.common`

### Chapter 16: The Class Library

#### 16.1.2 Overview of the Packages of the Standard Library

- ❌ The Java 11 Core Java SE API consists of the following modules and packages
- ✅ The Java **17** Core Java SE API consists of the following modules and packages

#### 16.4.6 Environment Variables of the Operating System

- ❌ static String getEnv(String name)
- ✅ static String get**e**nv(String name)

#### 16.6.1 Unix Time: January 1, 1970

- ❌ majority dropped from 24 to 18
- ✅ majority dropped from 2**1** to 18

#### 16.7.2 Human Time and Machine Time

- ❌ **From Chapter 7, Section 7.2.5, you learned how most classes are made for humans and that** only Instant/ Duration refers to machine time. 
- ✅ **Most classes are designed to represent human time;** only Instant and Duration deal with machine time.

#### 16.7.3 The LocalDate Date Class

- ❌ a number of years should be returned with minusYear(long, yearsToSubtract)
- ✅ a number of years should be returned with minusYear**s**(long, yearsToSubtract)

#### 16.8.2 Logging with java.util.logging

- ❌ src/main/java/com/tutego/insel/logging/CULDemo.java, JULDemo
- ✅ src/main/java/com/tutego/insel/logging/**J**ULDemo.java, JULDemo


### Chapter 17: Introduction to Concurrent Programming

#### Parameterizing Runnable

- ❌ Storing results from a background operation is more difficult than it might initially seem.
- ✅ **Returning** results from a background operation is more difficult than it might initially seem.

#### Rendezvous with join(...) *

- ❌ class java.lang.concurrent.TimeUnit
- ✅ class java.**util**.concurrent.TimeUnit

#### Threads with return via Callable

- ❌ In a separate class that extends Runnable
- ✅ In a separate class that **implements** Runnable

#### The stop() from the Outside and the Rescue with ThreadDeath

- ❌ class java.lang.TimeUnit implements Runnable
- ✅ *enum java.util.concurrent*.TimeUnit *extends Enum<TimeUnit> implements Serializable, Comparable<TimeUnit>*


### Chapter 18: Introduction to Data Structures and Algorithms

#### 18.1.3 The List Interface

- ❌ Whether or not the collection is empty is determined by isEmtpy().
- ✅ Whether or not the collection is empty is determined by isEm**pt**y().

#### 18.1.4 ArrayList

- ❌ The number of elements in the list (i.e., its size) is returned by the size() method**; the capacity of the underlying array is returned by capacity()**.
- ✅ The number of elements in the list (i.e., its size) is returned by the size() method.

#### 18.5 Creating a Stream > Table

- ❌ | Optional<T>	 | Stream()	  |  Stream<T> |
- ✅ | Optional<T>	 | **s**tream()	  |  Stream<T> |


### Chapter 19: Files and Data Streams

#### 19.2.1 FileSystem and Path

- ❌ A Path object can’t be created via a constructor like File because the class is abstract.
- ✅ A Path object can’t be created via a constructor like File because **Path is an interface**.

- ❌ final class java.nio.file.Path 
- ✅ **interface** java.nio.file.Path 

#### 19.2.2 The Files Utility Class > Easy Reading and Writing of Files

- ❌ Thus, already the second line of the program returns an exception **of the type** “java.nio.file.FileSystemNotFoundException: Provider 'http' not installed.”
- ✅ Thus, already the **first** line of the program returns an exception “java.nio.file.FileSystemNotFoundException: Provider 'http' not installed.”

#### 19.4.3 The Abstract Base Class InputStream

- ❌ Returns the number of available characters in the data stream
- ✅ Returns the number of available **bytes** in the data stream

- ❌ says nothing about how many characters the 
- ✅ says nothing about how many **bytes** the 

- ❌ Skips a number of characters. 
- ✅ Skips a number of **bytes**.

#### 19.4.5 The Appendable Interface*

- ❌ interface java.io.Appendable 
- ✅ interface java.**lang**.Appendable 

#### 19.4.7 The Interfaces Closeable, AutoCloseable, and Flushable

- ❌ 2 x extends AutoClosable
- ✅ 2 x extends AutoClo**e**sable

#### 19.5.1 Obtaining Byte-Oriented Data Streams via Files

- ❌ final abstract java.nio.file.Files 
- ✅ final abstract **class** java.nio.file.Files 


### Chapter 20: Introduction to Database Management with JDBC

#### 20.2.2 Accessing the Relational Database with Java

- ❌ // Access to FIRSTNAME, LASTNAME, STREET
- ✅ // Access to **ID, FIRSTNAME, LASTNAME**


### Chapter 21: Bits and Bytes, Mathematics and Money

#### Object Class Variables of the Math Class

- ❌ Object Variables of the Math Class
- ✅ **Class** Variables of the Math Class

- ❌ The Math class has two public class variables:
- ✅ The Math class has **three** public class variables:

#### The floorMod(...) Method to Round to Negative Infinity

- ❌ For this reason, besides a % b, the library method floorMod(a, b) is available, and the relationship between floorMod(...) and floorDiv(...) is floorDiv(a, b) * b + floorMod(a, b) == b.
- ✅ For this reason, besides a % b, the library method floorMod(a, b) is available, and the relationship between floorMod(...) and floorDiv(...) is floorDiv(a, b) * b + floorMod(a, b) == **a**.

- ❌ The completely different events (apart from the sign) in the pairs (+4, −3) and (−4, +3) simply result from different results of the division.
- ✅ The completely different **results** (apart from the sign) in the pairs (+4, −3) and (−4, +3) simply result from different results of the division.

#### The Largest and Smallest Values

- ❌ The classes Byte, Short, Integer, Long, Float, and Double have the constants MIN_VALUE and MAX_VALUE for their minimum and maximum value ranges.
- ✅ The classes Byte, Short, Integer, Long, Float, and Double have the constants MIN_VALUE and MAX_VALUE **representing the smallest and largest representable value of the respective type**.

#### Large Numbers*

- ❌ BigInteger for integers and BigDecimal for floats numbers, as shown in ...
- ✅ BigInteger for integers and BigDecimal for **decimal** numbers, as shown in ...

#### Creating BigInteger Objects

- ❌ The format string %4X fills the output on the left with zeros if necessary.
- ✅ The format string %**0**4X fills the output on the left with zeros if necessary.

#### Large Floats Decimal Numbers with BigDecimal

- ❌ Large Floats Numbers with BigDecimal
- ✅ Large **Decimal** Numbers with BigDecimal

#### Rounding Mode

- ❌ System.out.println( BigDecimal.ONE.divide(b) );
- ✅ System.out.println( BigDecimal.ONE.divide(**BigDecimal.TWO**) );


### Chapter 22: Testing with JUnit

#### 22.2.7 Testing Exceptions

- ❌ Listing 22.4 com/tutego/insel/junit/util**s**/StringsTest.java, reverse_null_string_1()
- ✅ Listing 22.4 com/tutego/insel/junit/util/StringsTest.java, reverse_null_string_1()


### Chapter 23: The Tools of the JDK

#### 23.3.1 Switches of the Java Virtual Machine

- ❌ As a simple number, n describes the bytes or kilobytes with an appended k or megabytes (appended m), for example, -Xms128m.
- ✅ As a simple number, n describes the bytes or kilobytes with an appended k or megabytes (appended m), for example, -Xm**x**128m.

