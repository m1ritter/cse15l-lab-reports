**Week 5 Lab Report**
# Researching Commands with find
**Monday, February 13, 2023**

By: Maddie Ritter

## -type & -remove
https://linuxhandbook.com/find-command-examples/
```
$ find . -type f -name "ch1.txt" -exec rm -f {} \;
```

```
$ find . -type f -name "chA.txt" -exec rm -f {} \;
```
I did this command with the skill-demo1-data directory open on my VS Code and was able to watch after hitting enter, the ch1.txt file in Abernathy was immediately deleted. The same happened for chA.txt in Castro. Both of these files were in writtem_2/non-fiction and although there was nothing on the terminal to indicate any change, I was able to observe the files were immediately deleted. 
The "-type f" indicated I am searching for a file, the "-name" indicates the name of hte file I want to delete ("ch1.txt" or "chA.txt") and the "-exec rm -f{}" indicates I want to remove the specified file. The single dot after "find" means current directory.
When I tried to search for the deleted files with "-name", nothing came up on the terminal indicated, again, that it worked!

I learned that the {} is an essential part of this command that you need to reference the result of the final command. The "\" and ";" are used together to terminal the exec command and escape the special character. 


## -delete
```
$ find . -name "ch2.txt" -delete
```
The command is a simplified version of the -remove above. Like -remove, it allows you to delete any file with the specified name in the current directory, indicated by the "." after find. In this case, I specified "ch2.txt" which is in the Abernathy directory, and after running this command, the file was immediately deleted. Much like -remove, there was no command-line output.

```
$ find . -name "ch3.txt" -delete
```
With this command, the "ch3.txt" file in Kauffman directory was immediately deleted as well! Again, there was no output to the terminal but I was able to watch the file delete quickly after my command. This is a much simpler and efficient command to use when wanting to delete a file, compared to the "-type, -name, -remove" command above.

## -empty
https://www.tecmint.com/35-practical-examples-of-linux-find-command/
```
$ find ./written_2 -empty
```

```
$ find ./written_2/non-fiction -empty
```
This command finds all of the emtpy directories or files that are specified at the terminal. Here, neither the directory, written_2 nor non-fiction have anything empty in them, so there is no output. 

## -size
https://linuxhandbook.com/find-command-examples/
```
find . -size -1G
```
```
// example output
./written_2
./written_2/non-fiction
./written_2/non-fiction/OUP
./written_2/non-fiction/OUP/Berk
./written_2/non-fiction/OUP/Berk/ch2.txt
./written_2/non-fiction/OUP/Berk/CH4.txt
...
```
The command "-size" is used to find files and directories that are a certain size. In this example I tried to find any files in the current directory that are smaller than 1GB (which is abbreviated with G in the command line). There was a lot! In the code block, I listed just a few that came up. Again, the "." after find represents the current directory, 

```
find . -size -20c
```
```
//example output 
./written_2/travel_guides
./written_2/travel_guides/berlitz1
./written_2/travel_guides/berlitz1/HandRLasVegas.txt
./written_2/travel_guides/berlitz1/HistoryJapan.txt
./written_2/travel_guides/berlitz1/IntroMalaysia.txt
./written_2/travel_guides/berlitz1/HandRIstanbul.txt
...
```
Similarly, for this one, I looked to find all the files that were bigger than 20 bytes (which is written as 20c at the command line). The output was almost identical to the first output showing that all of the files in written_2 are bigger than 20 bytes but smaller than 1 GB!
