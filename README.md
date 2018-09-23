# item-catalog
This web app is a project for the Udacity FSND Course.

## About
This project is a RESTful web application utilizing the Flask framework which accesses a SQL database that populates categories and their
items. OAuth2 provides authentication for further CRUD functionality on the application. Currently OAuth2 is implemented for Google Accounts.

##Skills
1. Python
2. HTML
3. CSS
4. Flask
5. OAuth

## instructions
1. install [vagrant](https://www.vagrantup.com/) and [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
2. Launch the Vagrant VM (vagrant up)
3. Log into Vagrant VM (vagrant ssh)
4. Navigate (cd vagrant/catalog/item-catalog)
5. The app imports requests which is not on this vm. Run sudo pip install requests
6. Run (python database_setup.py)
7. Run (python lotsofmenus)
8. Run (python project.py)
9. Go to [http://localhost:7777](http://localhost:7777)

## Create Google Sign in

1. Go to [Google Dev Console](https://console.developers.google.com/)
2. Sign up or Login if prompted
3. Go to Credentials
4. Select Create Crendentials > OAuth Client ID
5. Select Web application
6. Enter name 'Item-Catalog'
7. Authorized JavaScript origins = 'http://localhost:7777'
8. Select Create
9. Copy the Client ID and paste it into the data-clientid in login.html
10. On the Dev Console Select Download JSON
11. Rename JSON file to client_secrets.json
12. Place JSON file in item-catalog directory that you cloned from here
13. Run application using (python project.py)

## Creat facebook log in 
1. Go to [Facebook Developers](https://developers.facebook.com/)
2. Sign in to your account
3. create a new app
4. copy app id and paste it in fb_client_secrets.json/app_id
5. copy app secret and paste it in fb_client_secrets.json/app_secret
6. copy appid and paste it in login.html/appId
7. run (python project.py)
