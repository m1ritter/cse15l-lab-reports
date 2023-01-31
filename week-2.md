**Week 3 Lab Report**
# Servers and Bugs
**Monday, January 30, 2023**

By: Maddie Ritter

## **Part 1**
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {

    String string = "";
    
    public String handleRequest(URI url) {
        System.out.println("Path: " + url.getPath());
        if (url.getPath().contains("/add-message")) {
            String[] parameters = url.getQuery().split("=");
            if (parameters[0].equals("s")) {
                string += parameters[1] + "\n";
                return string;
            }
        }
        return "404 Not Found!";
    }
}
```
> /add-message?s=Hello
    
<img width="409" alt="Screen Shot 2023-01-29 at 8 11 40 PM" src="https://user-images.githubusercontent.com/122555675/215636399-ea7adb96-a1ee-4f42-b6e8-abae6101e57f.png"> <br> 

The handleRequest( ) method is called when a string is added to the URL. The method takes in arguments of type URI and the variable called 'string' gets elements added to it. For example, "Hello" is added after the /add-message?s=Hello request.<br> 
  
<br> 
> /add-message?s=How are you
       
<img width="502" alt="Screen Shot 2023-01-30 at 5 29 08 PM" src="https://user-images.githubusercontent.com/122555675/215637108-490cd9ec-94a2-42d1-a4eb-a1022d07529c.png">
The handleRequest( ) method is called. The method takes in an argument, url, that is of type URI and the variable 'string' is updated and returns both the first request (Hello) and the new request (How are you).



## Part 2 - reverseInPlace( )

**A failure inducing input**
```
public void testReverseInPlace() {
int[ ] input = { 1, 2, 3 };
ArrayExamples.reverseInPlace(input);

int[ ] result = { 3, 2, 1 };
assertArrayEquals(input, result);
}
```

**A non-failure inducing input**
```
public void testReverseInPlace() {
int[ ] input = { 1 };
ArrayExamples.reverseInPlace(input);

int[ ] result = { 1 };
assertArrayEquals(input, result);
}
```

**The Symptoms**

<img width="993" alt="image" src="https://user-images.githubusercontent.com/122555675/215297804-16e9d0d4-cf30-43fe-bac2-c34967e6b6cc.png">

**The Bug (Before + After)**
```
# Before the fix
static void reverseInPlace(int[] arr) {
  int[] newArr = new int[arr.length];
  
  for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```

```
# After the fix
static void reverseInPlace(int[] arr) {
  int[] newArr = new int[arr.length];
  
  for(int i = 0; i < arr.length; i++) {
      newArr[i] = arr[arr.length - i - 1];
    }
  for(int i = 0; i < arr.length; i++){
      arr[i] = newArr[i];
    }
  }
```
This fixes the bug because the issue with the initial code is that only half the array is getting copied and then the values in the second half get overwridden. So we needed to use the array copy again in order to store the rest of these values. 

## **Part 3**

In Lab 3, I learned about the important and usefulness of testing code. I had never really thought about a scenario where people could write testers that "pass," even though the code does not work properly. It is definitely a very useful skill to be able to write testers that fully assess what the code is meant to do, rather than "pass" under specific conditions. This is something I will look for and continue to approve upon moving forward. 


