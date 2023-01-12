# Week 1 Lab Report
## A Guide: Remote Computers & VS Code
**Monday, January 16, 2023**

By: Maddie Ritter

## *INSTALLING VS CODE:* 
Much like many of my fellow classmates, I already had VS Code downloaded to my mac. I opted to work on my computer rather than the lab computers since 
I am more familiar with the mac interface and my personal set up. I was able to get VS Code open rather quickly and clipped a quick screenshot! Here is 
the main window you should see when opening the code-editing application. 

<img width="1398" alt="Screen Shot 2023-01-12 at 8 15 10 AM" src="https://user-images.githubusercontent.com/122555675/212189980-021af8d0-9512-4974-afa6-450b4da18c09.png">


## *REMOTELY CONNECTING:*
Now here is the tricky bit. First you have to follow the link provided in the lab directions, and find yourself at a UCSD page that asks for your username (the first half of your email before @ucsd.edu) and your PID. From here, it gives you a special username beginning in "cs15lwi23." You then have to create a new password that will serve as your access to the remote computer. It takes approximately 15 minutes before the password is officially changed and can be used. Once this happens, you create a new terminal in VS code (top menu bar on desktop -> Terminal -> New Terminal). In the terminal we use the "ssh" key word (which stands for Secure Shell) to access the remote computer. I typed $ ssh (insert new username)@ieng6.ucsd.edu, which then prompted me to type my new password. Note: for security purposes, when you type your password the keys do not show up. 
Unfortunately, for me, after dozens of attempts, the terminal was not recognizing my password (this also happened to quite a few others). The TA suggested that I use my regular UCSD username to see if that worked. I again tried: m1ritter@ieng6.ucsd.edu and retyped my password when prompted. This finally worked! Below is a small screenshot of what I saw when I gained access to the remote computer.

<img width="414" alt="Screen Shot 2023-01-12 at 8 54 29 AM" src="https://user-images.githubusercontent.com/122555675/212192820-04e179d0-a736-4fc2-b7b4-90a40724442e.png">


## *TRYING SOME COMMANDS:*
From here, I began just playing around with some of the commands we learned in lecture. I didn't get to fancy with it since I am still learning about what they all mean and how they can be used. I used $ prep -l which was a command shown to me on the terminal itself when the remote computer connected. It gave more insight into the software packages that were available. I also used $ ls -a which seemed to list out all the folders in my directory. Below is a clip of some of these commands and their outputs.

<img width="1244" alt="Screen Shot 2023-01-12 at 8 57 26 AM" src="https://user-images.githubusercontent.com/122555675/212195713-f6b327be-e2b7-42d0-8811-29ce3f079244.png">

## From here, we did it! Successfully accessed the remote computer and practiced some of our software techniques and tools with VS code!
