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
<br>
Because of our new SSH key, no password was needed and it greatly expedited the logging in process! There was a quota error that spanned for dozens of lines that many students in my section got when logging in. The TAs cleared that it was okay to ignore this for the purpose of our lab, but the error is shown below!
<br>
<img width="768" alt="image" src="https://user-images.githubusercontent.com/122555675/220985393-c0aade74-3cd2-485e-8db5-33b32452a682.png">

## 5. Clone your fork of the repository from your Github account
`$ git clone git@github.com:ucsd-cse15l-w23/lab7.git <enter>` <br>
<br>
Because we have our handy SSH key and are logged into the server, we can use the SSH generated link provided on GitHub to clone our fork in the terminal. Below shows where the link was taken from, and what the code output was after running. <br>
<br>
<img width="1426" alt="image" src="https://user-images.githubusercontent.com/122555675/221434344-7e57d747-eb85-4742-8190-311d1834d3f4.png"> <br>
<br>
**Code Output** 
<br>
<img width="652" alt="image" src="https://user-images.githubusercontent.com/122555675/220984786-ade4e71a-7b18-48b9-92ce-2ed2f00634cd.png">

## 6. Run the tests, demonstrating that they fail
<img width="944" alt="image" src="https://user-images.githubusercontent.com/122555675/220986079-7df84593-9b4f-4977-9db0-7e883f8f6fc9.png">

Edit the code file to fix the failing test

Run the tests, demonstrating that they now succeed
Commit and push the resulting change to your Github account (you can pick any commit message!)

change to index2 at bottom
save
rerun
git add "ListExamples"
git commit -m "updated"
git push origin main
