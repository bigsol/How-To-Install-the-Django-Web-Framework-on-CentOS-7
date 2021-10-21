<h2>How To Install the Django Web Framework on CentOS 7</h2>

<h2>Install the EPEL Repository.</h2><br>

<p style="background-color:aqua">sudo yum install epel-release.</p>

<h2>Global Install from Packages</h2><br>

<p style="background-color:aqua">sudo yum install python-django.</p><br>

<h3>You can test that the installation was successful by typing:</h3><br>

<p style="background-color:aqua">django-admin --version</p>

<p style="background-color:aqua">1.11.27</p>


<h2>Global Install through pip</h2><br>

<h3>You can install pip from the EPEL repositories by typing:</h3><br>

<p style="background-color:aqua">sudo yum install python-pip</p>

<h3>Once you have pip, you can easily install Django globally by typing:</h3><br>

<p style="background-color:aqua">sudo pip install django</p>

  
<h2>Development Version Install through git</h2><br>

<p style="background-color:aqua">sudo yum install git python-pip/p>
  

<h2>Creating a Sample Project</h2><br> 



<h3>You can use the django-admin command to create a project:</h3>

<p style="background-color:aqua">django-admin startproject projectname</p>
<p style="background-color:aqua">cd projectname</p>  
  
<h3>To bootstrap the database (this uses SQLite by default) on more recent versions of Django, you can type:</h3>  

<p style="background-color:aqua">python manage.py migrate</p>

<h3>You can create an administrative user by typing:</h3><br>

<p style="background-color:aqua">python manage.py createsuperuser</p>


<h3>Once you have a user, you can start up the Django development server to see what a fresh Django project looks like. You should only use this for development purposes. Run:</h3><br>

<p style="background-color:aqua">python manage.py runserver 0.0.0.0:8000</p>

![image](https://user-images.githubusercontent.com/51197053/138260507-b3ed2399-623a-41ec-826f-9ff9d507d323.png)

<h3>Now, append /admin to the end of your URL to get to the admin login page:</h3>

<p style="background-color:aqua">server_ip_address:8000/admin</p>

![image](https://user-images.githubusercontent.com/51197053/138260780-9af7814f-ecca-4ba6-b720-0e63b37e59f4.png)

<h3>If you enter the admin username and password that you just created, you should be taken to the admin section of the site:</h3>


![image](https://user-images.githubusercontent.com/51197053/138260956-743a0340-3762-4854-b386-eba7e95d405c.png)

<text>  
  don't forget to add the line <p>ALLOWED_HOSTS = ['*'] </p>to the file setting and of course also disable FW or open port</text>
