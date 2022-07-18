Technic to use lambda added on java8 to generate the flow of data
Whole data -> mapping -> filtering -> filtering -> make result -> result

For now it is hard for me to understand the [whole document](https://futurecreator.github.io/2018/08/26/java-8-streams/)
However, I took the example code to sum the elements in the list

## Sum all the elements in the list
```java
int answer = divisor.stream().mapToInt(Integer::intValue).sum();   
```
