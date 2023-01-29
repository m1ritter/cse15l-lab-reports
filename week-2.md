**Week 2 Lab Report**
# Servers and Bugs
**Monday, January 30, 2023**

By: Maddie Ritter

## **Part 1**



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


## **Part 3**

In Lab 3, I learned about the important and usefulness of testing code. I had never really thought about a scenario where people could write testers that "pass," even though the code does not work properly. It is definitely a very useful skill to be able to write testers that fully assess what the code is meant to do, rather than "pass" under specific conditions. This is something I will look for and continue to approve upon moving forward. 


