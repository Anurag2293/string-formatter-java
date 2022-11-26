# StringFormat
# String and Integer Formatting with specified no. of Zeroes, spaces and Justification(Left or Right) 

````
import java.util.*;

public class FormatExample {  
    public static void main(String[] args) {          
        String str1 = String.format("|%d|", 101);  
        String str2 = String.format("|%10d|", 101);  // Specifying length of integer (default Right-Justification)
        String str3 = String.format("|%-10d|", 101); // Left-justifying within the specified width  
        String str4 = String.format("|% d|", 101);   
        String str5 = String.format("|%010d|", 101); // Filling with zeroes  
        
        System.out.println(str1);  
        System.out.println(str2);  
        System.out.println(str3);  
        System.out.println(str4);  
        System.out.println(str5);  
    }  
}  
````

Output:
````
|101|
|       101|
|101       |
| 101|
|0000000101|
````
