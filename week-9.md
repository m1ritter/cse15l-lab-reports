**Week 9 Lab Report**
# Researching Commands with grep!
**Monday, March 13, 2023**

By: Maddie Ritter

I had so much fun researching about commands to use with `find` in Week 5 that I decided to do it again this week with `grep`! I again used the file skill-demo1-data to do this activity! Let me walk you through what I discovered.

## Firstly, `grep -i "string" FILE`
https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/

This command is used to make insensitive searches for strings in a file. This is super important because if you are looking for the word "the" for example, "the" is often times used as the start of a sentence. It can also be used within sentences. The '-i' command makes it so the output will include both of these options, as well as all other posibilities: "THE", "tHE", "thE", etc... <br>

Here are some examples:
```
$ grep -i "ocean" WhereToItaly.txt
```
In this case, we see that there were no instances where "ocean" was used at the beginning of a sentence or capitalized.
<img width="616" alt="image" src="https://user-images.githubusercontent.com/122555675/224583797-efba834d-78e7-4b3e-81e9-240ff0e9d2db.png">


```
$ grep -i "try" WhereToItaly.txt
```
Here, we can see that the word "try" has been used in two different ways with different capitalization.
<img width="594" alt="image" src="https://user-images.githubusercontent.com/122555675/224583905-b9bf686a-90a7-4ff6-81c2-ea9c7d9dc5c4.png">



<br>
<br>

## Secondly, `grep -c "string" FILE`
https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/

This command allows you to count the number of lines that contains the given string or pattern. <br>

Here are a few examples:
```
$ grep -c "Italy" WhereToItaly.txt
```
In this case, the word "Italy" was found on 78 different lines.
<img width="622" alt="image" src="https://user-images.githubusercontent.com/122555675/224584319-df72fcbc-4912-449c-966e-c13f2f665fe9.png">

```
$ grep (-i) -r "rice" WhereToJapan.txt
```
Here, without using "-i" there were 21 lines where the word "rice" was found. I figured I would try it with "-i" and low and behold, there was one more additional line! <br>
<img width="645" alt="image" src="https://user-images.githubusercontent.com/122555675/224584412-5449b87c-500e-4492-8058-7a2b05679cff.png">



## Thirdly, `grep -c "string" FILE`
https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/

This command allows you to count the number of lines that contains the given string or pattern. <br>

Here are a few examples:
```
$ 
```

```
$ 
```

