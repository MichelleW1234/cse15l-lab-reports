# Step 1: Install VS Code.
   - Since I took CSE 11 previously, I already had VS Code installed, therefore I did not have to go through this step for this course. 
   - However, in order to install it, go to this link https://code.visualstudio.com/ , which should allow you to download a version according whatever operating system is being used.
   - Opening up VS Code, I was able to see this window:

![Screenshot1](https://user-images.githubusercontent.com/122498397/212212561-e6c64a37-35b2-46f0-b615-c6d7098efc22.jpg)

# Step 2: Remotely connecting.
   - To log into ieng6-202@ucsd.edu from my computer, I first went to the link https://sdacs.ucsd.edu/~icc/index.php to find my course-specific account.
   - Since I am a new student, in the corresponding boxed directly under "Forgot Username or New Student?", I input my last name and student ID with a lowercase "a" and then press "submit". This took me to a page with two account names--- one being a 12 digit sequence with "cs15lwi23" as the first 9 digits, which is the one I would use as my account username.

![Screenshot1](https://user-images.githubusercontent.com/122498397/212271877-eb881d4b-0c8b-42c8-adda-e0593aebb6a0.jpg)

![Screenshot2](https://user-images.githubusercontent.com/122498397/212271914-4e0c0de4-0628-45cd-a164-a28a699191ca.jpg)

   - I then clicked on that username, which took me to a page with a "change your password" button in blue.

![Screenshot3](https://user-images.githubusercontent.com/122498397/212271949-7a6c7d7b-1a98-4646-bf5f-8be65b5cfb40.jpg)

   - I clicked on that blue "change your password" button and, on the next page, entered in my account username and student ID again with a lowercase "a". After pressing "submit", this led me to the page that allowed me to change my password for this course specific account from my global account password (which is what it was by default) to a different password.

![Screenshot4](https://user-images.githubusercontent.com/122498397/212271989-d64a7ad8-d5ab-4972-945b-e95caa5c4970.jpg)

   - I entered my current password for my UCSD account and my new password (which must fit the guidelines to work) in their corresponding boxes. I also changed the dropdown option for the question "Change MyTritonLink password?" from Yes (the defualt) to No, preventing my UCSD global account from changing, and instead just my course-specific account. (NOTE: this is where I ran into a problem. Even though I didn't click "Check password" and did what the tutorial said, it still kept saying that my password didn't follow the guidelines. Eventually, I ended up copying and pasting a randomly generated password suggested by Google and pressed "Check Password", which finally ended up working and my password for my course account was changed.)
   - After waiting for a few minutes, I opened up VS code and entered 'ssh ACCOUNT_NAME@ieng6.ucsd.edu' into my terminal ('ACCOUNT_NAME' being my username).
   - I then entered my newly changed password for my account into the terminal. A message talking about "The authenticity of host 'ieng6.ucsd.edu" appeared, since it was my first time  connecting to the server, to which I entered yes as a response.
   - A message with my username appeared, indicating that I was logged into ieng6-202@ucsd.edu, along with a bunch of other information, such as the % CPU used on this system, Cluster status, and time and date of logging in.

![Screenshot2](https://user-images.githubusercontent.com/122498397/212212940-ddbc4098-235f-4bc8-bae1-6e77c7fbd6bd.jpg)

# Step 3: Trying Some Commands.
  - After I was logged in, I tried running some commands in the terminal, such as 'cd ~', 'cd', 'ls -lat', 'ls -a', and 'ls /home/linux/ieng6/cs15lwi23/ACCOUNT_USERNAME'. They came up with some interesting results.
  - I also tried running the commands 'cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/' and 'cat /home/linux/ieng6/cs15lwi23/public/hello.txt', however, since the file hello.txt didn't exist, I kept getting errors.
  - I was pretty confused by what some of the commands did and the results that popped up because of those commands, so hopefully I will learn more about them later on in this course.

![Screenshot3](https://user-images.githubusercontent.com/122498397/212213007-2f18722b-32b5-445e-911e-d0c1540dba5f.jpg)



