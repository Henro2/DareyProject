
<div style="text-align: center;">
  <span style="font-size: 40px; font-weight: bold;">Lemp Stack Implementation Project</span>
</div>



<span style="font-size: 20px;">-------------------------------------------------------------
</span>

<div style="text-align: center;">
  <span style="font-size: 20px; font-weight: bold;">STEP1</span>
</div>


- After connecting to my ubuntu instance via git bash, I updated my instance. 

- I installed **Nginx** using command (***Sudo apt install Nginx***)

After Nginx Installation, I checked to see if it was installed successfully using ***sudo systemctl status nginx*** . Its now in green and running 

![Alt text](images/nginxInstalled.png)

- To recieve traffic from our webserver (Nginx), I opened porth 80 (http) in my instance. With this, I will be able to access it via locally and via web browser. 

- To check local access , I used this command ***(curl http://localhost:80)***
 and it was successful 

![Alt text](<images/local access.png>)

-  To check access via web browser , I entered my AWS ubuntu instance public ip address on my browser, and it worked perfectly. 

![Alt text](images/webacess.png)




<div style="text-align: center;">
  <span style="font-size: 20px; font-weight: bold;">STEP2</span>
</div>

-  Installing **Mysql** : using ***Sudo apt install mysql-server -y***

- After installation of Mysql, I logged in successfully using  ***sudo mysql*** command


![Alt text](images/mysqlinstall.png)

- Now, while still in my database (mysql-server,) i changed root authentication methord to use mysql native password by entering this command ALTER USER **'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';** to use PassWord.1 as my password . Then, Exited **mysql**

-  
