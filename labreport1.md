# Week 1 Lab Report


Hello students!

This is a comprehensive guide on how to get started with cse15L. There will be three parts to this tutorial:

  1. Installing VsCode
  2. Remotely Connecting
  3. Trying some commands
---
**Installing VsCode**

Visit the VsCode website at [Visual Studio Code](https://code.visualstudio.com/). Read the instructions on how to install the program onto your computer, 
depending on which operating system you have (MacOS, Windows, etc).

<img width="437" alt="image" src="https://user-images.githubusercontent.com/122562133/215686040-954d60cc-2ebb-445c-b198-5ed51a818120.png">

For Mac, you should extract the file and drag it into your applications folder.

<img width="939" alt="image" src="https://user-images.githubusercontent.com/122562133/215693665-4a9e4bf1-d0c5-4ded-8d34-5a1fa15ee960.png">

From the applications folder, double click and click open when the warning prompt pops up.

<img width="287" alt="image" src="https://user-images.githubusercontent.com/122562133/215694002-82fd59ce-162c-4d9c-84ac-1a8339ca93b5.png">


When installed, open the Visual Studio Code app and you should see something like this:

![image](https://user-images.githubusercontent.com/122562133/212166001-27557b01-eba3-48f2-9243-5f42d07d8635.png)

You may have a different menu screen.


---
**Remotely Connecting**

If you are on Windows, you will need to install git at [Git for Windows](https://gitforwindows.org/).

Open a terminal in VSCode using 'Ctrl + `' (Command + ` for Mac users), or by using the Terminal tab. 

Run this command, replacing the zz with the letters in your account for this course. 

`ssh cs15lwi23zz@ieng6.ucsd.edu` 

Since it's your first time logging in, you may see something like this:

![image](https://user-images.githubusercontent.com/122562133/212165279-913830b1-3772-4adc-9cea-165f143baad5.png)

Type yes, then enter your password.

![image](https://user-images.githubusercontent.com/122562133/212166098-49fc5c34-365f-4fae-8bea-999fb96aaf4e.png)

You should see something like this once you have successfully logged in. You may have to wait a while, if you have just recently reset your password.
Well done! Your terminal is now connected to a computer in the CSE basement, and commands you run will run on that computer.

---
**Trying some commands**

Here are some commands for you to play around with:

- cd ~
- cd
- ls -lat
- ls -a
- ls <directory> where <directory> is /home/linux/ieng6/cs15lwi23/cs15lwi23abc, where the abc is one of the other group members’ username
- cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
- cat /home/linux/ieng6/cs15lwi23/public/hello.txt

  I got some interesting results. For example here is what happens when I type in ls -lat. From what it seems, it looks like it prints out all the files
  and the user associated to each one, while I was connected to the remote server.
  
  <img width="596" alt="image" src="https://user-images.githubusercontent.com/122562133/215689467-d67b920e-4169-496d-a7b5-a6a0973a5da7.png">

  
  
