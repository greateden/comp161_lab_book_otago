# Otago Uni COMP161 Lab Book
This is about the assignments listed in the Lab Book of COMP161 in the University of Otago. This book is mainly about JAVA programming.



## CONTENTS
- Chapter 1 [https://github.com/greateden/comp161_lab_book_otago#chapter-1]



## Chapter 1
>  不积跬步，无以至千里。 --老子《道德经》
>  
>  A journey of a thousand miles starts with a single step. - Lao Tzu, Tao Te Ching


### EXERCISE 1
```
error1:
Checker.java:10: error: class checker is public, should be declared in a file named checker.java
 public class checker{
        ^

error2:
There's no error, instead, the output changed from "abcd" to "efgh"

error3:
Checker.java:12: error: ';' expected
               System.out.println("blablabla")
                                              ^

error4:
 Checker.java:12: error: unclosed string literal
               System.out.println(blablabla");
                                           ^
                                           
error5:
 Checker.java:12: error: cannot find symbol
               System.out.println(blablabla);
                                  ^
   symbol:   variable blablabla
   location: class Checker

error f:
 Checker.java:12: error: package system does not exist
               system.out.println("blablabla");
                     ^
                     
errer g:
 Checker.java:12: error: cannot find symbol
               System.out.prntln("blablabla");
                         ^
   symbol:   method prntln(String)
   location: variable out of type PrintStream

error h:
  ----jGRASP exec: javac -g Checker.java
 Checker.java:13: error: reached end of file while parsing
        }
         ^

error i:
compile no problem, but when running, there's no main methods.
```


### EXERCISE 2
```java
/*
Encoding: UTF-8
Author: The Greatest Eden
Date:1 MAR 2023
Function: Show an address.
*/
public class Prog02{
       public static void main(String[ ] args){
              System.out.print("Ted Turner \n");
              System.out.println("66 Roundabout Drive");
              System.out.println("Dunedin 9011");
       }
}
```
**after changing:
 Ted Turner66 Roundabout DriveDunedin 9011**


### EXERCISE 3
```java
/*
Encoding: UTF-8
Author: The Greatest Eden
Date:1 MAR 2023
Function: Show a fucking joke.
*/

public class Joke{
       public static void main(String[ ] args){
              System.out.println("Q. What did the pirate say on his 80th birthday?");
              System.out.println("");
              System.out.println("A. AYA MATEY!");
       }
}
```


### EXERCISE 4
#### Correcting Errors 1
```java
/*
There should also be with comments!!!!!!!!
*/

public class PracticeExample1_1{
       public static void main(String[ ] args){
              System.out.psrintln("COMP161");
              System.out.println("18 points");
   }
}
```

#### Correcting Errors 1
```java
/*
blablabla
*/
public class PracticeExample2{
       public static void main(String[ ] args){
              char c = (char)67;
              System.out.println(c);
      }
}
```



## Chapter 2

### Important notes

#### Variable Naming Rules
> Class names should begin with a capital letter and use camel case. \
>`e.g. MyClassName`
>
> Variable and method names should begin with a lowercase letter and use camel case. \
>`e.g. myVariableName`
>
> Constants should be in all uppercase letters with words separated by underscores. \
>`e.g. MY_CONSTANT`
>
>Package names should be in all lowercase letters and use periods to separate words.\
> `e.g. com.mycompany.mypackage`
>
>Method names should be verbs or verb phrases that describe the action they perform \
> `e.g. getFirstName(), setLastName()`
>
>Boolean variables should be named with a prefix that indicates that they are booleans, such as "is" or "has" \
> `e.g. isFinished, hasChildren`
>
>Use meaningful and descriptive names for variables, methods, and classes.
>
>Avoid using abbreviations unless they are well-known or widely used in the domain.
>
>Use proper spelling and grammar in naming, even for internal variables and methods.
>
>Avoid using underscores in names unless it is for constants or naming conventions in existing code.

| Name | Valid? | Reason |
| ------ | ------ | ----- |
| Factorial | N | Start with capital | 
| aReallyQuiteExtremelyLongName | Y | 
| 3rdPlace | N | Start with digit | 
| floor27 | Y |  | 
| MAX_NUMBER | N | This is for consant not for variable | 
| gin&tonic | N | "&" connot be used when naming | 
| lowestBid$ | Y |  | 
| this | Y |  | 

#### Using “final" to initial value cannot be changed
#### String's "s" should be "S"
#### You can use `+= -= *= /=` in JAVA

### EXERCISE 1

> In Java, there are three types of comments:
> 
> **Single-line comment**
> 
> Single-line comments start with two forward slashes (//) and are used to explain a single line of code. Anything that follows the double slashes will be ignored by the compiler. These comments are generally used to provide short explanations of what the code is doing.
> Example:
> ```java
> // This is a single-line comment
> int x = 10; // This sets the value of x to 10
> ```
> 
> **Multi-line comments**
> 
> Multi-line comments start with a forward slash followed by an asterisk (/) and end with an asterisk followed by a forward slash (/). These comments are used to explain a block of code or to temporarily disable a block of code. Anything between the opening and closing symbols will be ignored by the compiler.
> Example:
> ```java
> /*
> This is a multi-line comment
> It can span multiple lines
> */
> 
> int x = 10; /* This sets the value of x to 10 */
> ```
> 
> **Javadoc comments**
> 
> Javadoc comments start with a forward slash followed by two asterisks (/) and end with an asterisk followed by a forward slash (*/). These comments are used to generate documentation for classes, methods, and variables. Javadoc comments can include special tags like @param, @return, and @throws that are used by documentation generators to provide information about a program's API.
> Example:
> ```java
> /**
> * This class represents a person
> * @author John Smith
> */
> public class Person {
>   private String name;
> 
>   /**
>   * Sets the person's name
>   * @param name The person's name
>   */
>   public void setName(String name) {
>     this.name = name;
>   }
> 
>   /**
>   * Gets the person's name
>   * @return The person's name
>   */
>   public String getName() {
>     return name;
>   }
> }
> ```
> 
> The key difference between these three types of comments is their purpose. Single-line and multi-line comments are used for code documentation and to make code more readable for developers. Javadoc comments, on the other hand, are used to generate API documentation that can be easily read by developers who are using your code.
> 
### EXERCISE 2

> **1 - c**
> 
> >  The value 78.9 is a floating-point literal, but the variable x is of type int, which can only hold integer values. The (int) before 78.9 is a type cast operator, which forces the compiler to convert the floating-point value to an integer value before assigning it to x.
After the cast, the fractional part of the value is truncated, and x will be assigned the integer value 78.
> 
> **2 - e,f**
> 
> **3 - a**
> 
> >  Comparing a and b, a declared a variable with the 'int' but b didnt.
> 
> **4 -g**
> 
> > The value 67 is cast to the char data type using the "(char)" syntax. The char data type in Java represents a single character, such as a letter, digit, or symbol, and can be initialized with either a Unicode value or a character literal enclosed in single quotes.
In this case, the Unicode value 67 represents the character 'C', so the variable "c" will be assigned the value 'C'.
> 
> **5 -d**
> 
> **6 -b** 
> 
> > no "string" before "name", so the variable "name" has already been declared
> 
> **7 - h**

### EXERCISE 3

> `main`. That’s a entry point and main logic of the program, it can _call_ other methods too if the programmer want it do that and there’s no bug.
> 
> `2 plus 2 is 22`
> 
> This is because it is using string concatenation. In Java, the + operator is used for both addition and string concatenation. When the + operator is used with two strings, it concatenates them to form a new string. When it is used with a string and a number, the number is first converted to a string and then concatenated with the original string.
> 
> In the given statement, the first string is "2 plus 2 is ". Then, the + operator is used with the number 2, which is first converted to a string "2", and concatenated to the previous string, producing "2 plus 2 is 2". Finally, the + operator is again used with the number 2, which is also converted to a string "2", and concatenated to the previous string, producing "2 plus 2 is 22". 
> 
> `40 is the new thirty`
> 
> This is because the statement is evaluated from left to right, following the order of operations. In this case, the addition operator + is used with two numbers 20 and 20, which results in the integer 40. Then, the + operator is used with the string " is the new thirty.", which is concatenated to the integer 40 to form the final string "40 is the new thirty.".

### EXERCISE 4

> The value of i will be 50, and the value of x will also be 50.

