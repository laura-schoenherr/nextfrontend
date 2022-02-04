# Project setup 

### installing keycloak

Download Keycloak

First step is to download and extract
[keycloak-16.1.0.zip](https://github.com/keycloak/keycloak/releases/download/16.1.0/keycloak-16.1.0.zip) 
from the Keycloak website.

After extracting you should have a directory named keycloak-16.1.0.

### Start keycloak

From a terminal open the directory keycloak-16.1.0, then to start Keycloak run the following command.

On Linux run:
```
bin/standalone.sh
```

On Windows run:
```
bin\standalone.sh
```

### Create an admin user

Keycloak does not come with a default admin user, which means before you can start using Keycloak you need to create an admin user.

To do this open <http://localhost:8080/auth>, then fill in the form with your preferred username and password.

### Login to the admin console
Go to the Keycloak Admin Console and login with the username and password you created earlier.

### Create a realm
* Hover your mouse over the dropdown in the top-left corner where it says ```Master``` 
then click on ```Add Realm```
* Fill in the form with the following values: 
  * Name: ```myrealm``` (choose your preferred realm name)
* Click ```Create```

### Create a user 

There is no user in the realm you just created, so you need to create one: 
1. Click ```Users``` in the left-hand menu
  * Click ```Add user``` in the top-right corner of the table
2. Fill in the form with the following values
    * Username: ````yourPreferredName````
    * First Name: your first name
    * Last Name: your last name
3. Click ```Save```

The user needs an initial password to log into the application. To create one do this: 

1. Click ```Credentials``` on the top of the page
2. Fill in the ```Set Password``` form with a password of your choice
3. Click ```ON``` next to ```Temporary``` to prevent having to update 
the password on the first login. The button must then turn grey and show ```OFF```.

### Secure the app




## Project setup yarn
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
