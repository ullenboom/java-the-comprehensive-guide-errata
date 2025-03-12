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

#### Array Lengths Are Final

- ❌ The **object variable attribute** length of an array isn’t only public and of type int, but of course also final
- ✅ The **instance variable** length of an array isn’t only public and of type int, but of course also final


### Chapter 5: Handling Characters and Strings

#### Is That So?

- ❌ The term “letter” not only describes well-known letters like “a” or “α.” Unicode contains more about than 100,000 characters, including hundreds of letters.
- ✅ The term “letter” not only describes well-known letters like “a” or “α.” Unicode contains more about than **150,000** characters, including hundreds of letters **from different languages**.

#### Strings

- ❌ A string is a collection of characters **(data type char)** that the runtime environment stores in the memory in an orderly fashion
- ✅ A string is a collection of characters that the runtime environment stores in the memory in an orderly fashion

#### Escape Sequences _(in Text Blocks)_

- ❌ This text block becomes the string "1\u0002". 
- ✅ This text block becomes the string **"1\n2"**.

#### Other Options for Decomposition

- ❌ “
- ✅ "

#### Creating String Objects with Constructors and from Repeats

- ❌ `isAnangram`
- ✅ `isAnagram`

#### Default Methods in the CharSequence Interface

- ❌ This interface has two default methods:
- ✅ This interface has **three** default methods:

#### Pimp My String with Format Specifiers

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


### Chapter 9: There Must Be Exceptions

#### Exceptions in Java with try and catch

- ❌ The `try block` is usually  followed by a catch block ... 
- ✅ The `try` is usually  followed by a catch block ... 

- ❌ Program code that can execute an exception
- ✅ Program code that can **raise** an exception


### Chapter 10: Nested Types

#### Non-Static Nested Types

- ❌ Let’s declare an inner class named Room in House with the following example code:
- ✅ Let’s declare an inner class named **Coconut** in **AlmondJoy** with the following example code:

#### Creating Instances of Inner Classes

- ❌ To create an object in the static main(String[]) method of the house, you can write the following code:
- ✅ To create an object **of type Coconut** in the static main(String[]) method of the **class AlmondJoy**, you can write the following code:


### Chapter 11: Special Types of Java SE

#### Sequence of Comparators

- ❌ Let’s now use these thenComparing(...) methods from Comparator in an example that sorts a list of names last name and then by first name.
- ✅ Let’s now use these thenComparing(...) methods from Comparator in an example that sorts a list of **calories and name**.


### Chapter 12: Generics<T>

#### Quite by Chance One or the Other Argument

- ❌ In the following example, T in sit(...) doesn’t refer to the parameter variable of the Lupilu class, but does refer to the parameter value of the method:
- ✅ In the following example, T in sit(...) doesn’t refer to the parameter variable of the Lupilu **interface**, but does refer to the parameter value of the method:

#### Generics Aren’t Covariant, but Invariant

- ❌ Then, p.set(2.2) isn’t OK, for example, because Double isn’t compatible with Integer.
- ✅ Then, **r**.set(2.2) isn’t OK, for example, because Double isn’t compatible with Integer.

#### Bounded Wildcards

- ❌ All possible Number objects can be in the rocket p.
- ✅ All possible Number objects can be in the rocket **r**.

#### Type Tokens

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

(none)


### Chapter 16: The Class Library

#### Overview of the Packages of the Standard Library

- ❌ The Java 11 Core Java SE API consists of the following modules and packages
- ✅ The Java **17** Core Java SE API consists of the following modules and packages

#### Environment Variables of the Operating System

- ❌ static String getEnv(String name)
- ✅ static String get**e**nv(String name)

#### Logging with java.util.logging

- ❌ src/main/java/com/tutego/insel/logging/CULDemo.java, JULDemo
- ✅ src/main/java/com/tutego/insel/logging/**J**ULDemo.java, JULDemo


### Chapter 17: Introduction to Concurrent Programming

#### Parameterizing Runnable

- ❌ Storing results from a background operation is more difficult than it might initially seem.
- ✅ **Returning** results from a background operation is more difficult than it might initially seem.

#### Rendezvous with join(...) *

- ❌ class java.lang.concurrent.TimeUnit
- ✅ class java.**util**.concurrent.TimeUnit


### Chapter 18: Introduction to Data Structures and Algorithms

#### Creating a Stream / Table

- ❌ | Optional<T>	 | Stream()	  |  Stream<T> |
- ✅ | Optional<T>	 | **s**tream()	  |  Stream<T> |


### Chapter 19: Files and Data Streams

#### FileSystem and Path

- ❌ A Path object can’t be created via a constructor like File because the class is abstract.
- ✅ A Path object can’t be created via a constructor like File because **Path is an interface**.

- ❌ final class java.nio.file.Path 
- ✅ **interface** java.nio.file.Path 

#### Easy Reading and Writing of Files

- ❌ Thus, already the second line of the program returns an exception **of the type** “java.nio.file.FileSystemNotFoundException: Provider 'http' not installed.”
- ✅ Thus, already the **first** line of the program returns an exception “java.nio.file.FileSystemNotFoundException: Provider 'http' not installed.”

#### The Appendable Interface*

- ❌ interface java.io.Appendable 
- ✅ interface java.**lang**.Appendable 

#### Obtaining Byte-Oriented Data Streams via Files

- ❌ final abstract java.nio.file.Files 
- ✅ final abstract **class** java.nio.file.Files 


### Chapter 20: Introduction to Database Management with JDBC

(none)


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

(none)


### Chapter 23: The Tools of the JDK

#### Switches of the Java Virtual Machine

- ❌ As a simple number, n describes the bytes or kilobytes with an appended k or megabytes (appended m), for example, -Xms128m.
- ✅ As a simple number, n describes the bytes or kilobytes with an appended k or megabytes (appended m), for example, -Xm**x**128m.

