# Otago Uni COMP161 Lab Book
This is about the assignments listed in the Lab Book of COMP161 in the University of Otago. This book is mainly about JAVA programming.

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
              System.out.println("COMP161");
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
