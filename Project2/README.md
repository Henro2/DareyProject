# Git project <!DOCTYPE html>
<html>
<head>
    <style>
        p {
            color: blue;
        }
    </style>
</head>
<body>
    <p>  </p>
</body>
</html>



1. I made a new directory called <font color="green">**Project2**</font> using <font color="red">**mkdir**</font> Command

2. I then switch my working directory to <font color="yellow">**Project2**</font> i just created

3. I initialized it using the <font color="brown">**Init**</font> command . Check bellow image

![Alt text](Images/1.png)

4. Inside my new directory <font color="red">**Project2**</font>, I created a filed called <font color="red">**index.txt**</font>.

In GUI, i  then wrote this text "my commit" in <font color="blue">**index.txt**</font> file 

With <font color="red">**Git add .**</font> command, I added my file <font color="red">**index.txt**</font> file to be tracked.  and them commited using commit command **commit  -m** "(message)"

![Alt text](Images/2.png)

5. I made a new branch called <font color="red">**mainedited**</font> using **git checkout -b**

and it swiched authomatically to the new branch 

![Alt text](Images/3.png)

6. I listed the all the branched using <font color="red">**git branch**</font> command


![Alt text](Images/4.png)

7. I edited the content of this file called  <font color="red">**index.txt**</font> so i can merge it to the <font color="red">**main**</font> branch 

  <font color="red">**add .**</font> to track the file 
 <font color="red">**commit -m** </font>(to comit)

 <font color="red">**git checkout main**</font> to switch to main branch

 <font color="red">**git merge**</font> (mainedited) to merge 

![Alt text](Images/5.png)

8.  <font color="red">**git branch -d**</font> deleted this branch **mainedited**


