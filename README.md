# SubStrings_of_String

## Introduction
This Java program prints all possible substrings of a given string. It demonstrates the use of nested loops and the built-in `substring()` method to extract and print substrings.

## Code Overview
```java
package subString;

public class SubStrings_of_String
{
    public static void main(String[] args)
    {
        String str = "abc";
        System.out.println("All substrings of '" + str + "':");
        for (int i = 0; i < str.length(); i++)
        {  
            for (int j = i + 1; j <= str.length(); j++)
            {  
                System.out.println(str.substring(i, j));  
            }  
        }  
    }
}
```

## Explanation of Code

### **Package Declaration**
```java
package subString;
```
- The program is part of the `subString` package, which helps in organizing classes logically.

### **Class Declaration**
```java
public class SubStrings_of_String
```
- The class `SubStrings_of_String` contains the `main` method and executes the logic to generate substrings.

### **Main Method**
```java
public static void main(String[] args)
```
- The entry point of the Java program where execution starts.

### **Variable Declaration**
```java
String str = "abc";
```
- A string variable `str` is initialized with the value "abc". This is the input string from which substrings will be generated.

### **Printing Statement**
```java
System.out.println("All substrings of '" + str + "':");
```
- Prints the heading indicating that substrings of the given string will be displayed.
- Uses string concatenation to dynamically include the value of `str` in the output.

### **Outer for Loop**
```java
for (int i = 0; i < str.length(); i++)
```
- The outer loop sets the starting index of the substring.
- It starts from `0` and runs until `i < str.length()`, ensuring all characters are considered.

### **Inner for Loop**
```java
for (int j = i + 1; j <= str.length(); j++)
```
- The inner loop determines the ending index of the substring.
- It starts from `i + 1` (ensuring at least one character is present in the substring) and goes up to `str.length()`.

### **Substring Extraction and Printing**
```java
System.out.println(str.substring(i, j));
```
- Extracts a substring from index `i` (inclusive) to `j` (exclusive) using the built-in `substring()` method.
- Prints each substring on a new line.

## **Built-in Methods Used**
1. **`substring(int start, int end)`**
   - Extracts a substring from the given string.
   - The `start` index is inclusive, and `end` is exclusive.
2. **`length()`**
   - Returns the length of the string.
   - Used in the loop condition to ensure the loop iterates correctly.
3. **`println()`**
   - Prints the output to the console.

## **Output of the Program**
```
All substrings of 'abc':
a
ab
abc
b
bc
c
```

## **Time Complexity**
- The program uses nested loops, making the time complexity **O(n²)**, where `n` is the length of the string.

## **Conclusion**
This program effectively generates all possible substrings of a string using nested loops and Java's `substring()` method. Understanding this concept is useful in string manipulation, pattern matching, and data processing tasks.

## Clone
```
git clone https://github.com/Ananthadatta02/Java-SubString_To_String.git
```
