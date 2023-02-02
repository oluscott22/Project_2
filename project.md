## LEMP STACK IMPLEMENTATION


### **create a new instance for project 2 and ssh into the instance**

![New Instance](./Images/Second%20Instance.png)

![Second Instance Terminal](./Images/Second%20Instance%20terminal.png)


### **INSTALLING THE NGINX WEB SERVER**



`sudo apt update`

`sudo apt install nginx`

`sudo systemctl status nginx`

![nginx status](./Images/nginx.png)


#### **Welcome to nginx**

![Welcome to nginx](./Images/welcome%20to%20nginx.png)

### **INSTALLING MYSQL**

`sudo apt install mysql-server`

`sudo mysql`

![Welcome to MYSQL](./Images/Welcome%20to%20MYSQL.png)

`sudo mysql_secure_installation`

![All Done](./Images/ALL%20Done.png)



**Test if you’re able to log in to the MySQL console by typing**

`sudo mysql -p`

![Login to mysql](./Images/login%20mysql.png)


.[Database management system](https://en.wikipedia.org/wiki/Database#Database_management_system)


.[Relational database](https://en.wikipedia.org/wiki/Relational_database)





### **INSTALLING PHP**

`sudo apt install php-fpm php-mysql`

![PHP](./Images/PHP%201.png)

**Below screenshot shows the PHP version installed**

![PHP Version](./Images/PHP%20version.png)

.[PHP](https://www.php.net/)


### **CONFIGURING NGINX TO USE PHP PROCESSOR**

`sudo mkdir /var/www/projectLEMP`

`sudo chown -R $USER:$USER /var/www/projectLEMP`

`sudo nano /etc/nginx/sites-available/projectLEMP`

`sudo ln -s /etc/nginx/sites-available/projectLEMP /etc/nginx/sites-enabled/`

`sudo nginx -t`

![nginx -t](./Images/nginx%20-t.png)

`sudo unlink /etc/nginx/sites-enabled/default`


### **TESTING PHP WITH NGINX**

`sudo nano /var/www/projectLEMP/info.php`

![last screen](./Images/last%20Screen.png)

`sudo rm /var/www/your_domain/info.php`






