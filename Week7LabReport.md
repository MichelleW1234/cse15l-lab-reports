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

### Keys pressed:

### commands summary:
- `ssh cs15lwi23aov@ieng6.ucsd.edu`

## 5. Clone your fork of the repository from your Github account

### Screenshot:

### Keys pressed:

### commands summary:
- `git clone git@github.com:MichelleW1234/lab7.git`
  
## 6. Run the tests, demonstrating that they fail
  
### Screenshot:

### Keys pressed:

### commands summary:
- `cd lab7`
- `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`
- `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`
  
## 7. Edit the code file to fix the failing test
  
### Screenshot:

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

### Keys pressed:

### commands summary:
- `git add .`
- `git commit -m "changed index2 to index1 in ListExamples.java"`
- `git push`
 
  
