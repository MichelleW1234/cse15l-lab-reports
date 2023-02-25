For the lab report this week, reproduce the task from the competition on your own. 
For each numbered step starting right after the timer (so steps 4-9), take a screenshot, 
and write down exactly which keys you pressed to get to that step. 
For special characters like <enter> or <tab>, write them in angle brackets with code formatting. 
Then, summarize the commands you ran and what the effect of those keypresses were.

For example:
  
when you run the tests, you might want to use the up arrow or Ctrl-R to access your bash history 
rather than typing in the full command with classpath, etc. 
You might say something like this accompanying the screenshot for running the tests:

Keys pressed: <up><up><up><up><enter>, <up><up><up><up><enter>

The javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java command was 4 up in the search history, 
so I used up arrow to access it. 
Then the java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore command was 4 up in the history, 
so I accessed and ran it in the same way.
  
# Steps:
## 1. (Setup) Delete any existing forks of the repository you have on your account
## 2. (Setup) Fork the repository
## 3. (The real deal) Start the timer!
## 4. Log into ieng6

### Screenshot:
  
![screenshot1](https://user-images.githubusercontent.com/122498397/221346142-69f347a0-6d32-437b-bdb4-53af398090b6.jpg)

### Keys pressed:

### commands summary:
- `ssh cs15lwi23aov@ieng6.ucsd.edu`

## 5. Clone your fork of the repository from your Github account

### Screenshot:
  
![screenshot2](https://user-images.githubusercontent.com/122498397/221346153-5f94be46-437d-4056-8fd2-fa3eff27f6f0.jpg)

### Keys pressed:

### commands summary:
- `git clone git@github.com:MichelleW1234/lab7.git`
  
## 6. Run the tests, demonstrating that they fail
  
### Screenshot:
  
![screenshot3](https://user-images.githubusercontent.com/122498397/221346185-7157452a-2470-4c76-a024-1c004df69b22.jpg)

### Keys pressed:

### commands summary:
- `cd lab7`
- `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`
- `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`
  
## 7. Edit the code file to fix the failing test
  
### Screenshot:
  
![screenshot4](https://user-images.githubusercontent.com/122498397/221346201-ab6f350b-2083-4519-84e1-2a7fa7c8ec77.jpg)

### Keys pressed:
- `<down>` x 42
- `<right>` x 12
- `<backspace>`
- `<2>`
- `<ctrl>` + `<o>`
- `<enter>`
- `<ctrl>` + `<x>`

### commands summary:
- `nano ListExamples.java`
- `ctrl + o`
- `ctrl + x`
  
## 8. Run the tests, demonstrating that they now succeed
  
### Screenshot:
  
![screenshot5](https://user-images.githubusercontent.com/122498397/221346217-857b592e-43de-474a-b9a8-f598fbcab611.jpg)

### Keys pressed:
- `<up>` x 2
- `<enter>`
- `<up>` x 4
- `<enter>`

### commands summary:
- `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`
- `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`
  
## 9. Commit and push the resulting change to your Github account
  
### Screenshot:
  
![screenshot6](https://user-images.githubusercontent.com/122498397/221346231-666db3c5-f3ad-42b5-a3bc-33dc504e203e.jpg)

### Keys pressed:

### commands summary:
- `git add .`
- `git commit -m "changed index2 to index1 in ListExamples.java"`
- `git push`
 
  
