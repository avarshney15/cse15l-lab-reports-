# Lab Report 3
The topic for this lab report will be the linux command, find. I will teach you how to use find in 4 different and very interesting ways as well as tell you about my experience at each step. To help you better understand the steps I will include screenshots as well.
## -D
This option is very useful to find 
```
skill-demo1-data:269$ find written_2 -type d
    written_2
    written_2/non-fiction
    written_2/non-fiction/OUP
    written_2/non-fiction/OUP/Abernathy
    written_2/non-fiction/OUP/Berk
    written_2/non-fiction/OUP/Castro
    written_2/non-fiction/OUP/Fletcher
    written_2/non-fiction/OUP/Kauffman
    written_2/non-fiction/OUP/Rybczynski
    written_2/travel_guides
    written_2/travel_guides/berlitz1
    written_2/travel_guides/berlitz2
```
In this example, the type command helped find all of the directories in written_2. It showed us all of the sub-rirectories as well.
```
:non-fiction:283$ find OUP -type f    
    OUP/Abernathy/ch1.txt
    OUP/Abernathy/ch14.txt
    OUP/Abernathy/ch15.txt
    OUP/Abernathy/ch2.txt
    OUP/Abernathy/ch3.txt
    OUP/Abernathy/ch6.txt
    OUP/Abernathy/ch7.txt
    OUP/Abernathy/ch8.txt
    OUP/Abernathy/ch9.txt
    OUP/Berk/CH4.txt
    OUP/Berk/ch1.txt
    OUP/Berk/ch2.txt
    OUP/Berk/ch7.txt
    OUP/Castro/chA.txt
    OUP/Castro/chB.txt
    OUP/Castro/chC.txt
    OUP/Castro/chL.txt
    OUP/Castro/chM.txt
    OUP/Castro/chN.txt
    OUP/Castro/chO.txt
    OUP/Castro/chP.txt
    OUP/Castro/chQ.txt
    OUP/Castro/chR.txt
    OUP/Castro/chV.txt
    OUP/Castro/chW.txt
    OUP/Castro/chY.txt
    OUP/Castro/chZ.txt
    OUP/Fletcher/ch1.txt
    OUP/Fletcher/ch10.txt
    OUP/Fletcher/ch2.txt
    OUP/Fletcher/ch5.txt
    OUP/Fletcher/ch6.txt
    OUP/Fletcher/ch9.txt
    OUP/Kauffman/ch1.txt
    OUP/Kauffman/ch10.txt
    OUP/Kauffman/ch3.txt
    OUP/Kauffman/ch4.txt
    OUP/Kauffman/ch5.txt
    OUP/Kauffman/ch6.txt
    OUP/Kauffman/ch7.txt
    OUP/Kauffman/ch8.txt
    OUP/Kauffman/ch9.txt
    OUP/Rybczynski/ch1.txt
    OUP/Rybczynski/ch2.txt
    OUP/Rybczynski/ch3.txt
```
In this example, "-type f" was used to find all of the files in the folder, including the ones in all of the sub directories. 
I found this command by searching on google and then finding this [website](https://www.computerhope.com/unix/ufind.htm).
## -Printf
This command helps us print useful information such as the path, owner or size of each file in a directory.
```
:OUP:303$ find Berk -printf "%p\n"
Berk
Berk/CH4.txt
Berk/ch1.txt
Berk/ch2.txt
Berk/ch7.txt
```
In this example, we used -printf to print the path of each file in the Berk directory. This was specified in "%p\n". 
```
:OUP:304$ find Berk -printf "%u\n"
cs15lwi23awr
cs15lwi23awr
cs15lwi23awr
cs15lwi23awr
cs15lwi23awr
```
In this example, we find the user who owns all of the files in the Berk directory. As we are running the command on the ieng6 account and ahve downloaded the directory, cs15lwi23awr is shown as the owner for all these files. 
I found this command by searching on google and then finding this [website](https://www.computerhope.com/unix/ufind.htm).

##  -Mtime 
This command finds the files modified in a certain number of days in a directory.
```
non-fiction:327$ find OUP -mtime -7              
OUP
OUP/Abernathy
OUP/Abernathy/ch1.txt
OUP/Abernathy/ch14.txt
OUP/Abernathy/ch15.txt
OUP/Abernathy/ch2.txt
OUP/Abernathy/ch3.txt
OUP/Abernathy/ch6.txt
OUP/Abernathy/ch7.txt
OUP/Abernathy/ch8.txt
OUP/Abernathy/ch9.txt
OUP/Berk
OUP/Berk/CH4.txt
OUP/Berk/ch1.txt
OUP/Berk/ch2.txt
OUP/Berk/ch7.txt
OUP/Castro
OUP/Castro/chA.txt
OUP/Castro/chB.txt
OUP/Castro/chC.txt
OUP/Castro/chL.txt
OUP/Castro/chM.txt
OUP/Castro/chN.txt
OUP/Castro/chO.txt
OUP/Castro/chP.txt
OUP/Castro/chQ.txt
OUP/Castro/chR.txt
OUP/Castro/chV.txt
OUP/Castro/chW.txt
OUP/Castro/chY.txt
OUP/Castro/chZ.txt
OUP/Fletcher
OUP/Fletcher/ch1.txt
OUP/Fletcher/ch10.txt
OUP/Fletcher/ch2.txt
OUP/Fletcher/ch5.txt
OUP/Fletcher/ch6.txt
OUP/Fletcher/ch9.txt
OUP/Kauffman
OUP/Kauffman/ch1.txt
OUP/Kauffman/ch10.txt
OUP/Kauffman/ch3.txt
OUP/Kauffman/ch4.txt
OUP/Kauffman/ch5.txt
OUP/Kauffman/ch6.txt
OUP/Kauffman/ch7.txt
OUP/Kauffman/ch8.txt
OUP/Kauffman/ch9.txt
OUP/Rybczynski
OUP/Rybczynski/ch1.txt
OUP/Rybczynski/ch2.txt
OUP/Rybczynski/ch3.txt
```
Over here, the files above have been modified in the last seven days as they ahve been downloaded in the last seven days. 
```
:non-fiction:328$ find OUP -mtime +7

```
This command is supposed to find all of the files that have been modified more than 7 days ago. It cannot find any files as all the files have been downloaded less than a week ago. 
I found this command by asking ChatGPT about the various ways in which the find command can be used in a linux system. 

## -maxdepth
This option helps one search for a specific type of file only certain levels deep from the startign directory.
```
non-fiction:334$ find OUP -maxdepth 2 -name "*.txt"
OUP/Abernathy/ch1.txt
OUP/Abernathy/ch14.txt
OUP/Abernathy/ch15.txt
OUP/Abernathy/ch2.txt
OUP/Abernathy/ch3.txt
OUP/Abernathy/ch6.txt
OUP/Abernathy/ch7.txt
OUP/Abernathy/ch8.txt
OUP/Abernathy/ch9.txt
OUP/Berk/CH4.txt
OUP/Berk/ch1.txt
OUP/Berk/ch2.txt
OUP/Berk/ch7.txt
OUP/Castro/chA.txt
OUP/Castro/chB.txt
OUP/Castro/chC.txt
OUP/Castro/chL.txt
OUP/Castro/chM.txt
OUP/Castro/chN.txt
OUP/Castro/chO.txt
OUP/Castro/chP.txt
OUP/Castro/chQ.txt
OUP/Castro/chR.txt
OUP/Castro/chV.txt
OUP/Castro/chW.txt
OUP/Castro/chY.txt
OUP/Castro/chZ.txt
OUP/Fletcher/ch1.txt
OUP/Fletcher/ch10.txt
OUP/Fletcher/ch2.txt
OUP/Fletcher/ch5.txt
OUP/Fletcher/ch6.txt
OUP/Fletcher/ch9.txt
OUP/Kauffman/ch1.txt
OUP/Kauffman/ch10.txt
OUP/Kauffman/ch3.txt
OUP/Kauffman/ch4.txt
OUP/Kauffman/ch5.txt
OUP/Kauffman/ch6.txt
OUP/Kauffman/ch7.txt
OUP/Kauffman/ch8.txt
OUP/Kauffman/ch9.txt
OUP/Rybczynski/ch1.txt
OUP/Rybczynski/ch2.txt
OUP/Rybczynski/ch3.txt
```
Over here, the find command goes only two levels deep in the directory and finds all of the text files.

```
:non-fiction:335$ find OUP -maxdepth 1 -name "*.txt"

```
Over here, I have given the same command with the max depth set as 1. Since there are only subdirectories and no text files at the first level this query gave us no results.
I found this command by asking ChatGPT about the various ways in which the find command can be used in a linux system. 

Hope you understood everything in this blog post!


