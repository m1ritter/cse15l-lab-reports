**Week 7 Lab Report**
# Done Quick
**Monday, February 27, 2023**

By: Maddie Ritter

## 1. Setup Delete any existing forks of the repository you have on your account
Rather than deleting the entire repo from my account, the TAs suggest to simply delete the directory and start again that way. 
That is what I show here! 
<br>
`$ cd .. <enter>` <br>
`$ rm -rf lab7 <enter>` <br>
`$ ls <enter>`

<img width="664" alt="Screen Shot 2023-02-23 at 9 30 42 AM" src="https://user-images.githubusercontent.com/122555675/220984556-26b89a32-7392-4bf4-b35a-882f75c0be19.png">

## 2. Setup Fork the repository
Here, I made a fork of the repository for the first time! I used the link provided in the writeup to take me to the Lab 7 repository. From here, I used the "Fork" tab in the top right corner (shown below) in order to "create a new fork." In the example below, I have already forked the repository. 

<img width="1427" alt="image" src="https://user-images.githubusercontent.com/122555675/220985203-0da2c1df-9570-4ab6-8411-eb30da58e26a.png">

## 3. The real deal Start the timer!

## 4. Log into ieng6
`$ ssh m1ritter@ieng6.ucsd.edu <enter>`

Because of our new SSH key, no password was needed and it greatly expedited the logging in process! There was a quota error that spanned for dozens of lines that many students in my section got when logging in. The TAs cleared that it was okay to ignore this for the purpose of our lab, but the error is shown below!

<img width="768" alt="image" src="https://user-images.githubusercontent.com/122555675/220985393-c0aade74-3cd2-485e-8db5-33b32452a682.png">

## 5. Clone your fork of the repository from your Github account
`$ git clone git@github.com:ucsd-cse15l-w23/lab7.git <enter>` <br>
`$ cd lab7 <enter>` <br>

Because we have our handy SSH key and are logged into the server, we can use the SSH generated link provided on GitHub to clone our fork in the terminal. Below shows where the link was taken from, and what the code output was after running. <br>

<img width="1426" alt="image" src="https://user-images.githubusercontent.com/122555675/221434344-7e57d747-eb85-4742-8190-311d1834d3f4.png"> <br>
<br>

**Code Output** 
<br>
<img width="652" alt="image" src="https://user-images.githubusercontent.com/122555675/220984786-ade4e71a-7b18-48b9-92ce-2ed2f00634cd.png">

## 6. Run the tests, demonstrating that they fail
`$ <up><up><up><enter>`
`$ <up><up><enter>`

The *javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java* was three up in the search history so I used the up arrow to find it and then pressed enter to run it. Similarly, the javac command was two up arrows away so I found it and hit enter to run.

<img width="963" alt="image" src="https://user-images.githubusercontent.com/122555675/221478553-141aa489-1120-4341-aa19-0a13d64bae3a.png">

## 7. Edit the code file to fix the failing test
``
``

<img width="1307" alt="image" src="https://user-images.githubusercontent.com/122555675/221478026-6e77485b-4d02-4931-88c7-4b6075bfd288.png">

## 8. Run the tests, demonstrating that they now succeed

<img width="957" alt="image" src="https://user-images.githubusercontent.com/122555675/221477594-d8b483b6-ad6e-4c00-9240-1803a6a81c91.png">


## 9. Commit and push the resulting change to your Github account (you can pick any commit message!)

<img width="845" alt="image" src="https://user-images.githubusercontent.com/122555675/221480248-93d81646-015f-4a17-aec7-bfb28def64af.png">

git add "ListExamples"
git commit -m "updated"
git push origin main
