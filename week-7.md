**Week 7 Lab Report**
# Done Quick
**Monday, February 27, 2023**

By: Maddie Ritter

## 4. Log into ieng6

`$ ssh m1ritter@ieng6.ucsd.edu <enter>`

Because of our new SSH key, no password was needed and it greatly expedited the logging in process! There was a quota error that spanned for dozens of lines that many students in my section got when logging in. The TAs cleared that it was okay to ignore this for the purpose of our lab, but the error is shown below!

<img width="768" alt="image" src="https://user-images.githubusercontent.com/122555675/220985393-c0aade74-3cd2-485e-8db5-33b32452a682.png">

## 5. Clone your fork of the repository from your Github account

`$ git clone <cmnd V> <enter>` <br>
`$ cd lab7 <enter>` <br>

Because we have our handy SSH key and are logged into the server, we can use the SSH generated link provided on GitHub to clone our fork in the terminal. Below shows where the link was taken from, and what the code output was after running. I copied the link using the little box icon on the right and pasted the link in the terminal. Then I changed my directory to be lab7. <br>

<img width="1426" alt="image" src="https://user-images.githubusercontent.com/122555675/221434344-7e57d747-eb85-4742-8190-311d1834d3f4.png"> <br>
<br>

**Code Output** 
<br>
<img width="652" alt="image" src="https://user-images.githubusercontent.com/122555675/220984786-ade4e71a-7b18-48b9-92ce-2ed2f00634cd.png">

## 6. Run the tests, demonstrating that they fail
`$ <up><up><up><enter>`
`$ <up><up><enter>`

The 'javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java' was three up in the search history so I used the up arrow to find it and then pressed enter to run it. Similarly, the javac command was two up arrows away so I found it and hit enter to run.

<img width="963" alt="image" src="https://user-images.githubusercontent.com/122555675/221478553-141aa489-1120-4341-aa19-0a13d64bae3a.png">

## 7. Edit the code file to fix the failing test
`$ <up><up><up><enter>` to find `$ nano ListExamples.java`
Once in nano:
`$ <down><down><down>....` to find and change index1 to index2
`$ <cmnd o><enter>` to save
`$ <cmnd x><enter>` to exit nano

<img width="1307" alt="image" src="https://user-images.githubusercontent.com/122555675/221478026-6e77485b-4d02-4931-88c7-4b6075bfd288.png">

## 8. Run the tests, demonstrating that they now succeed
`$ <up><up><enter>` to find and run the javac Junit command
`$ <up><up><up><up><enter>`to find the java command to run the Junit command

<img width="957" alt="image" src="https://user-images.githubusercontent.com/122555675/221477594-d8b483b6-ad6e-4c00-9240-1803a6a81c91.png">


## 9. Commit and push the resulting change to your Github account (you can pick any commit message!)
`$ <up><up><up><up><up><up><enter>` to find `$ git add ListExamples.java`
`$ <up><up><up><up><up><enter>` to find the `$ git commit -m "updated"`
`$ <up><up><up><up><enter>` to find the `$ git push origin main`

<img width="754" alt="image" src="https://user-images.githubusercontent.com/122555675/221721215-20005250-6d8c-4dbe-a807-705ad3c34f7c.png">

