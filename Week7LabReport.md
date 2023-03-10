# Challenge Tasks:
## Steps:
### 1. (Setup) Delete any existing forks of the repository you have on your account
### 2. (Setup) Fork the repository
### 3. (The real deal) Start the timer!
### 4. Log into ieng6

#### Screenshot:
  
![screenshot1](https://user-images.githubusercontent.com/122498397/221346142-69f347a0-6d32-437b-bdb4-53af398090b6.jpg)

#### Keys pressed:
- `<cmd>` + `<v>`
- `<enter>`

#### commands summary:
I pasted the command `ssh cs15lwi23aov@ieng6.ucsd.edu` into the terminal after copying it from my notes by pressing `<cmd>` and `<v>` together, and then pressed `<enter>` to complete the login process.

### 5. Clone your fork of the repository from your Github account

#### Screenshot:
  
![screenshot2](https://user-images.githubusercontent.com/122498397/221346153-5f94be46-437d-4056-8fd2-fa3eff27f6f0.jpg)

#### Keys pressed:
- `<g>`
- `<i>`
- `<t>`
- `<space>`
- `<c>`
- `<l>`
- `<o>`
- `<n>`
- `<e>`
- `<space>`
- `<cmd> + <v>`
- `<enter>`

#### commands summary:
I first typed in the command `git clone`, and then pasted the SSH link of the lab7 repository on Github by pressing `<cmd>` and `<v>` together, creating the command `git clone git@github.com:MichelleW1234/lab7.git`. I then pressed `<enter>` to clone the repository. 
  
### 6. Run the tests, demonstrating that they fail
  
#### Screenshot:
  
![screenshot3](https://user-images.githubusercontent.com/122498397/221346185-7157452a-2470-4c76-a024-1c004df69b22.jpg)

#### Keys pressed:
- `<c>`
- `<d>`
- `<space>`
- `<l>`
- `<a>`
- `<b>`
- `<7>`
- `<enter>`
- `<cmd> + <v>`
- `<enter>`
- `<cmd> + <v>`
- `<space>`
- `<l>` + `<shift>`
- `<i>`
- `<s>`
- `<t>`
- `<e>` + `<shift>`
- `<x>`
- `<a>`
- `<m>`
- `<p>`
- `<l>`
- `<e>`
- `<s>`
- `<t>` + `<shift>`
- `<e>`
- `<s>`
- `<t>`
- `<s>`
- `<enter>`

#### commands summary:
I first entered the command `cd lab7` to get into the lab7 directory and access the `ListExamplesTest.java` file. I then pasted the command `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` after copying it from my notes by pressing `<cmd> and <v>` together, and pressed `<enter>` to go forth with compiling the tests. Finally, I pasted `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore` after copying it from my notes by pressing `<cmd> and <v>` together, and completed the command by typing in the name of the tester file without the `.java` at the end (`ListExamplesTests`), which created the command `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`. I pressed `<enter>` to run the tester file. 
  
### 7. Edit the code file to fix the failing test
  
#### Screenshot:
  
![screenshot4](https://user-images.githubusercontent.com/122498397/221346201-ab6f350b-2083-4519-84e1-2a7fa7c8ec77.jpg)

#### Keys pressed:
- `<n>`
- `<a>`
- `<n>`
- `<o>`
- `<space>`
- `<l>` + `<shift>`
- `<i>`
- `<s>`
- `<t>`
- `<e>` + `<shift>`
- `<x>`
- `<a>`
- `<m>`
- `<p>`
- `<l>`
- `<e>`
- `<s>`
- `<.>`
- `<j>`
- `<a>`
- `<v>`
- `<a>`
- `<enter>`
- `<down>` x 42
- `<right>` x 12
- `<backspace>`
- `<2>`
- `<Ctrl>` + `<o>`
- `<enter>`
- `<Ctrl>` + `<x>`

#### commands summary:
I first typed the command `nano ListExamples.java` in order to edit the  `ListExamples.java` to fix the issue that caused the tests in `ListExamplesTests.java` to fail, and then pressed `<enter>`. I found the issue (the last `index1` in the bottom-most while-loop should've been `index2`), and was able to get the the error and fix it by pressing `<down>` 42 times, `<right>` 12 times, `<backspace>` (to delete the `1` in `index1`), and `<2>` (to change it to `index2`). I then pressed `Ctrl and o` together and hit `<enter>` in order to save the change in `ListExamples.java`. Finally, I pressed `Ctrl + x` together to exit out of the file and return to the terminal. 
  
### 8. Run the tests, demonstrating that they now succeed
  
#### Screenshot:
  
![screenshot5](https://user-images.githubusercontent.com/122498397/221346217-857b592e-43de-474a-b9a8-f598fbcab611.jpg)

#### Keys pressed:
- `<up>` x 2
- `<enter>`
- `<up>` x 4
- `<enter>`

#### commands summary:
I compiled the tests in `ListExamplesTests.java` once more using the compiling command `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`, which I accessed in my history by pressing `<up>` 2 times and hitting `<enter>`. I then ran the tests with the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` command by pressing `<up>` 4 times and hitting `<enter>`. This time, all the tests passed!
  
### 9. Commit and push the resulting change to your Github account
  
#### Screenshot:
  
![screenshot6](https://user-images.githubusercontent.com/122498397/221346231-666db3c5-f3ad-42b5-a3bc-33dc504e203e.jpg)

#### Keys pressed:
- `<g>`
- `<i>`
- `<t>`
- `<space>`
- `<a>`
- `<d>`
- `<d>`
- `<space>`
- `<.>`
- `<enter>`
- `<g>`
- `<i>`
- `<t>`
- `<space>`
- `<c>`
- `<o>`
- `<m>`
- `<m>`
- `<i>`
- `<t>`
- `<space>`
- `<->`
- `<m>`
- `<space>`
- `<">`
- `<c>`
- `<h>`
- `<a>`
- `<n>`
- `<g>`
- `<e>`
- `<d>`
- `<space>`
- `<i>`
- `<n>`
- `<d>`
- `<e>`
- `<x>`
- `<1>`
- `<space>`
- `<t>`
- `<o>`
- `<space>`
- `<i>`
- `<n>`
- `<d>`
- `<e>`
- `<x>`
- `<2>`
- `<space>`
- `<i>`
- `<n>`
- `<space>`
- `<l>` + `<shift>`
- `<i>`
- `<s>`
- `<t>`
- `<e>` + `<shift>`
- `<x>`
- `<a>`
- `<m>`
- `<p>`
- `<l>`
- `<e>`
- `<s>`
- `<.>`
- `<j>`
- `<a>`
- `<v>`
- `<a>`
- `<">`
- `<enter>`
- `<g>`
- `<i>`
- `<t>`
- `<space>`
- `<p>`
- `<u>`
- `<s>`
- `<h>`
- `<enter>`

#### commands summary:
I first typed in the command `git add .` and pressed `<enter>` to add my edits in `ListExamples.java` to the lab7 repository on Github from my computer. I then typed the command `git commit -m "changed index2 to index1 in ListExamples.java"` and pressed `<enter>` to commit my edit on Github with the commit message "changed index2 to index1 in ListExamples.java". Finally, I typed in the command `git push` and hit `<enter>` to upload the content to the remote repository.
  
