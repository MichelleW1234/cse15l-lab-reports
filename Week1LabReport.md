You will write a tutorial for incoming 15L students (and your future self!) about how to log into a course-specific account on ieng6. Your post should include the steps you took, along with screenshots of what each step looked like. You’re free to use the screenshots you took for lab 1, or new ones. Complete any steps you didn’t complete in your group on your own.

Overall, make sure you have at least 3 screenshots, one for each of the steps below (though more is useful, remember that this will help out your future self). For each step include 2-3 sentences or bullet points describing what you did. If for some reason you didn’t do the step exactly, describe why not (maybe your computer already had something on it, maybe the department computers worked differently, etc).

Installing VScode
Remotely Connecting
Trying Some Commands

Step 1: Install VS Code.
   - Since I took CSE 11 previously, I already had VS Code installed, therefore I did not have to go through this step for this course. 
   - However, in order to install it, go to this link https://code.visualstudio.com/ , which should allow you to download a version according whatever operating system is being used.
   - Opening up VS Code, I was able to see this window:

![Screenshot1](https://user-images.githubusercontent.com/122498397/212212561-e6c64a37-35b2-46f0-b615-c6d7098efc22.jpg)

Step 2: Remotely connecting.
   - To log into ieng6-202@ucsd.edu from my computer, I first went to the link https://sdacs.ucsd.edu/~icc/index.php to find my course-specific account.
   - Since I am a new student, in the corresponding boxed directly under "Forgot Username or New Student?", I input my last name and student ID with a lowercase "a" and then press "submit". This took me to a page with two account names--- one being a 12 digit sequence with "cs15lwi23" as the first 9 digits, which is the one I would use as my account username.
   - I then went back to the previous page, and, in the corresponding boxes directly under "Account Lookup", entered in my username and student ID with a lowercase "a" and then press "submit". This lead me to a page with a "change your password" button in blue.
   - I clicked on that blue "change your password" button and, on the next page, entered in my account username and student ID again with a lowercase "a". After pressing "submit", this led me to the page that allowed me to change my password for this course specific account from my global account password (which is what it was by default) to a different password.
   - I entered my current password for my UCSD account and my new password (which must fit the guidelines to work) in their corresponding boxes. 
   - I changed the dropdown option for the question "Change MyTritonLink password?" from Yes (the defualt) to No, preventing my UCSD global account from changing, and instead just my course-specific account. (NOTE: this is where I ran into a problem. Even though I didn't click "Check password" and did what the tutorial said, it still kept saying that my password didn't follow the guidelines. Eventually, I ended up copying and pasting a randomly generated password suggested by Google and pressed "Check Password", which finally ended up working and my password for my course account was changed.)
   - After waiting for a few minutes, I opened up VS code and entered ssh ACCOUNT_NAME@ieng6.ucsd.edu into my terminal (ACCOUNT_NAME being my username).
   - I then entered my newly changed password for my account into the terminal. A message talking about "The authenticity of host 'ieng6.ucsd.edu" appeared, since it was my first time  connecting to the server, to which I entered yes as a response.
   - A message with my username appeared, indicating that I was logged into ieng6-202@ucsd.edu, along with a bunch of other information, such as the % CPU used on this system, Cluster status, and time and date of logging in.

![Screenshot2](https://user-images.githubusercontent.com/122498397/212212940-ddbc4098-235f-4bc8-bae1-6e77c7fbd6bd.jpg)

Step 3: Trying Some Commands.
  - After I was logged in, I tried running some commands in the terminal, such as cd ~, cd, ls -lat, ls -a, and ls /home/linux/ieng6/cs15lwi23/ACCOUNT_USERNAME. They came up with some interesting results.
  - I also tried running the commands cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/ and cat /home/linux/ieng6/cs15lwi23/public/hello.txt, however, sibce the file heelo.txt didn't exist, I kept getting errors.
  - I was pretty cunfused by what some some of the commands did and what popped up because of those commands, so hopefully I will learn more about them later on in this course.

![Screenshot3](https://user-images.githubusercontent.com/122498397/212213007-2f18722b-32b5-445e-911e-d0c1540dba5f.jpg)



