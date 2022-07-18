##String

It was not possible to string += char, so found another method by format in String method

```java
String threeString = String.format("%c%c%c",s.charAt(i-2),s.charAt(i-1),s.charAt(i)); // create string adding chars
```

##Change datatype
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