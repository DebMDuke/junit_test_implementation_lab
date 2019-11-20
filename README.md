# JUnit Test Implementation lab
Practice writing JUnit tests for a project specification by first implementing a test for a simple calculator class.
This small example shows you how to write a unit test. 
## Create the class under test

Create a new file `Calculator.java` and copy the following code to this file.

```java
public class Calculator {
  public int evaluate(String expression) {
    int sum = 0;
    for (String summand: expression.split("\\+"))
      sum += Integer.valueOf(summand);
    return sum;
  }
}
```

Now save this class:

    javac Calculator.java


## Create a test

Create a new Junit 4 test file `CalculatorTest.java` and copy the following code to this file.

```java
import static org.junit.Assert.assertEquals;
import org.junit.Test;

public class CalculatorTest {
  @Test
  public void evaluatesExpression() {
    Calculator calculator = new Calculator();
    int sum = calculator.evaluate("1+2+3");
    assertEquals(6, sum);
  }
}
```
Run the test as a JUnit test.

  

## Let the test fail

Modify `Calculator.java` in order to get a failing test. Replace the line

    sum += Integer.valueOf(summand);

with

    sum -= Integer.valueOf(summand);

and save the class.



Now rerun the test class to see that it fails and the output is

    JUnit version 4.12
    .E
    Time: 0,007
    There was 1 failure:
    1) evaluatesExpression(CalculatorTest)
    java.lang.AssertionError: expected:<6> but was:<-6>
      at org.junit.Assert.fail(Assert.java:88)
      ...
    
    FAILURES!!!
    Tests run: 1,  Failures: 1

JUnit tells you which test failed (`evaluatesExpression(CalculatorTest)`) and what went wrong:

    java.lang.AssertionError: expected:<6> but was:<-6>

### Now Write the JUnit test for a class
##Here's a description of the Class MyBook
MyBook has five String fields: title, authorFirstName, authorLastName, and two forms of identifiers isbn10 and isbn13.  Design the class so that individual instances never contain null fields. 

MyBook class has two constructors. The default constructor sets the title, authorFirstName, and authorLastName fields to the string, "None Given” and both isbn10 and isbn13 to a String containing all zeroes. The overloaded constructor has five String parameters and initializes title, authorFirstName, authorLastName, isbn10, and isbn13 with these values. 

Use this method header for the parameterized constructor:
public MyBook(String title, String authorFirstName, String authorLastName, String isbn10, String isbn13)

Implement accessor (getter) and mutator (setter) methods for each of the instance variables. In addition, define the equals method that inherits from Object.

In this lab you'll be implementing the JUnit test class for the MyBook class.
