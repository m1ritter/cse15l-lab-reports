**Week 5 Lab Report**
# Researching Commands with find
**Monday, February 13, 2023**

By: Maddie Ritter

## -type & -remove
```
$ find . -type f -name "ch1.txt" -exec rm -f {} \;
```

```
$ find . -type f -name "ch1.txt" -exec rm -f {} \;
```
I did this command with the skill-demo1-data directory open on my VS Code and was able to watch after hitting enter, the ch1.txt file in Abernathy was immediately deleted. The same happened for chA.txt in Castro. Both of these files were in writtem_2/non-fiction and although there was nothing on the terminal to indicate any change, I was able to observe the files were immediately deleted. 

## -empty
```
$ find ./written_2 -empty
```

```
$ find ./written_2/non-fiction -empty
```
This command finds all of the emtpy directories or files that are specified at the terminal. Here, neither the directory, written_2 nor non-fiction have anything empty in them, so there is no output. 
