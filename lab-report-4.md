# Lab Report 4
The topic for this lab report will cover steps 4 to 9 from lab 7. To help you better understand the steps I will include screenshots as well.
## Step 4: Log in to ieng6
Keys Pressed: "<up><enter>"
The line with my ssh and my ieng6 remote account username was one line above so I went one up and pressed enter. As I had set up the SSH key I did not have to input my password. ![image](log-in-lab-7.png)

## Step 5: Clone your fork of the repository from your Github account
Keys Pressed: "<up><up><up><up><up><up><up><up><up><up><up><up><up><enter>"
The line with the command for cloning the lab 7 repository from git hub, git clone https://github.com/avarshney15/lab7, was 13 lines up so I went up and pressed enter. This created a clone of the git repository in my ieng6 account. ![image](git-command.png)

## Step 6: Run the tests, demonstrating that they fail
Keys Pressed: "<c><d>< ><l><a><b><7>, <up><up><up><up><up><up><up><up><up><Enter>"
I first used th cd command to enter the new lab 7 directory. Then I went 9 commands up to find the, javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java, command which compiles all of the java files in the folder. Then I went 9 commands up to get the  java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests command and pressed enter which runs the ListExamplesTests class and outputs the result. As you can see, the tests are failing right now. ![image](error.png)

## Step 7: Edit the code file to fix the failing test

