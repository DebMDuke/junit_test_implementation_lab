# JUnit Test Implementation lab
Practice writing JUnit tests for a project specification

Here's a description of the project:
Class MyBook has five String fields: title, authorFirstName, authorLastName, and two forms of identifiers isbn10 and isbn13.  Design the class so that individual instances never contain null fields. 
MyBook class has two constructors. The default constructor sets the title, authorFirstName, and authorLastName fields to the string, "None Given” and both isbn10 and isbn13 to a String containing all zeroes. The overloaded constructor has five String parameters and initializes title, authorFirstName, authorLastName, isbn10, and isbn13 with these values. The MyBook class will be graded using a jUnit test class, so the order of the parameters needs to match. Use this method header for the parameterized constructor:
public MyBook(String title, String authorFirstName, String authorLastName, String isbn10, String isbn13)

Implement accessor (getter) and mutator (setter) methods for each of the instance variables. In addition, define the following methods:
•	public boolean equals(Object otherBook)
•	public String toString()
The equals method overrides the one that is inherited from the Object class, therefore the method signature must match exactly – the parameter must be of type Object. Two books are equal if they have the same ISBN numbers.  Guidelines for overriding the equals method:
•	Use the == operator to check if the argument is a reference to itself.
•	Use the instanceof operator to check if the argument has the correct data type.
•	Cast the argument to the correct type.
•	For each significant data member, test for equality.
•	Test these three properties: 
o	Is it symmetric?  
o	Is it transitive?  
o	Is it consistent?

In this lab you'll be implementing the JUnit test class for the MyBook class.
