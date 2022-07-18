## String

It was not possible to string += char, so found another method by format in String method
```java
String threeString = String.format("%c%c%c",s.charAt(i-2),s.charAt(i-1),s.charAt(i)); // create string adding chars
```

## Character

Check if each char of the string is a digit
```java
String s = "TargetString01"
for (int i=0; i<s.length(); i++){
    char each_char = s.charAt(i);
    if (Character.isDigit(each_char)){
        ...
    }
}
```
*otherwise*
```java
for(char each_char : s.toCharArray()){ // .toCharArray() is optional but error might occur without
    if (Character.isDigit(each_char)){
    ...
    }
}
```

Slicing the string
```java
String s = "TargetString01"
System.out.println(s.substring(1)) // "argetString01"
System.out.println(s.substring(1,3)) // "ar" as inclusive start, exclusive end
```

## Array

Create another array according to the original array
```java
int [] original_array = {1,2,3,4,5};
int [] array_copyof = Arrays.copyOf(original, 3); // {1, 2, 3}
int [] array_copyoofrange = Arrays.copyOfRange(original, 3, 5}; // {4, 5} as again, inclusive start, exclusive end
```

## ArrayList

Create a blank ArrayList - no need to define the length, but if you want, put the initial length in parenthesis
```java
ArrayList<Integer> divisor = new ArrayList<Integer>(); // (10) will make 10 length arrayList
divisor.add("Hello");   // divisor == ["Hello"]
divisor.add("Hello");   // divisor == ["Hello", "Hello"]

divisor.set(1, "World"); // divisor == ["Hello", "World"]

divisor.remove("Hello"); // divisor == ["World"]
divisor.remove(0) // divisor == []

divisor.clear(); // clear all the elements in the ArrayList

int num_divisor = divisor.size(); // ArrayLists uses size() not length
```

## HashSet *NEW*

similar to set (e.g (3,4,5)) in python not accepting duplicates
```java
// // Convert array to HashSet in Java
// import java.io.*;
// import java.util.Iterator;
// Importing Set libraries
import java.util.Set;
import java.util.HashSet;

Set<Integer> unique = new HashSet<>(); // create a new HashSet
for (int element : nums){               // for each element in nums array
    unique.add(element);                // add it to the new HashSet - then only unique values remain in HashSet
    }
int unique_ponkemon = unique.size();    // HashSet uses size() not length
```


## Change datatype

String to Integer
```java
int answer_integer = Integer.parseInt(answer_string);
```
Integer to String
```java
String answer_string = Integer.toString(answer_integer)
```
Integer to Long
```java
Long answer_long = Long.valueOf(answer_integer)
```
