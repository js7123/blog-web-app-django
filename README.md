# blog-app-django
Blog application using Django and SQLite

## Prerequisites
Prior to running the server please provide Django secret key value in blogsite\blogsite\settings.py file :
```
SECRET_KEY = '<django-secret-key>'
```
## Instructions
1. Create a virtual environment.
    Sample command:
    ```
    py -m venv <virtual environment name>
    ```
2. Activate the virtual environment.
   Sample command (for Linux or macOS environment):
   ```
   source <virtual environment name>\Scripts\activate
   ```
   Sample command (for Windows environment):
   ```
   .\<virtual environment name>\Scripts\activate
   ```
4. Checkout the project from Github to a local directory.
5. As mention in the prerequisites section, prior to running the server please provide Django secret key value in the *blogsite\blogsite\settings.py* file :
   ```
   SECRET_KEY = '<django-secret-key>'
   ```
5. Create a sample superuser. Sample command:
   ```
   <your directory>\blogsite>python manage.py createsuperuser
   ```
   Provide desired username, email address and password.

6. Start the server. Sample command:
   ```
   <your directory>\blogsite>python manage.py runserver 127.0.0.1:8089
   ```
7. For examples of the activities supported by this blog web application please see *"Site Administration"*, *"Adding a blog post"* and *"Viewing blog posts"* sections below.
    
## Site Administration
For site administration purposes please open the following link in your browser:
```
http://127.0.0.1:8089/admin
```
Site adminitration allows you to add and modify users and group users. It also allows the administrator to remove user blog posts.

## Adding a blog post
To create a log the user must login first and then click on the **+ Add** link displayed in the **BLOG/Posts** section. Next the blog form displayed must be completed and the **"SAVE"** button must be selected.

## Viewing blog posts
To create a log the user must login first and then use the following link to the **blog** page:
```
http://127.0.0.1:8089/blog/
```
Please notice that only blogs having "Published" Status can be viewed in that page.


