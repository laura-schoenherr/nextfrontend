# nextfrontend

##  before Project setup 

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



## Project setup
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
