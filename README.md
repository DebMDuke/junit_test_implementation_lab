# junit_test_implementation_lab
Practice writing JUnit tests for a project specification

Suppose that you've been given the following project to write a Java class called CustomDate that represents a simple date consisting of a month, day, and year.  It has three data fields of type int to represent the date.  For example, July 4, 1776, is month 7, day 4, and year 1776.  
*	Write a default, parameterless constructor that sets the CustomDate to January 1, 2000 and parameterized constructor with three arguments
*	Write setter methods (setDay, setMonth, setYear) with a single argument to change the day month or year
*	Implement getter methods (getDay, getMonth, getYear) that return the day, month, or year as an int
*	Implement a private method to check the validity of the CustomDate object (private boolean isValidDate( ) )
*	Write a method to determine whether the current year is a leap year (public boolean isLeapYear ( ) )
*	Include an method to change the current date by one day (public void advanceOneDay ( ) )
*	Include an method to change the current date by one week (public void advanceOneWeek ( ) )
*	Override the toString method inherited from Object (public String toString () ) 
*	Override the equals method inherited from Object (public boolean equals (Object obj) ) 
*	Implement a method that compares this CustomDate object with the object passed as a parameter for chronological order and returns a negative integer, zero, or a positive integer, if this object is less than, equal to, or greater than the specified object. (public int compareTo (Object obj) ). For example, 
A year is a leap year if it is divisible by 4 but not by 100.  If the year is divisible by 100, it is a leap year only if it is also divisible by 400.

In this lab you'll be implementing the JUnit test class for the CustomDate class.
