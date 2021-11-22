# Cinema Shop
This application shows my skills in Java, Spring, REST, SOLID principles, CRUD.  
### Tecnologies
Hibernate, Spring(Core, Web, Security), MySQL, Tomcat, JSON. 
## Let's install some programs:
- Install Tomcat [9.0.50](https://tomcat.apache.org/download-90.cgi)
  . Don't recommend installing version 10+ because program may not work correctly.
- Install [mySQL workbench](https://dev.mysql.com/downloads/workbench/).
- Install [Postman](https://web.postman.co/) for sending http requests.

## Run application:
For ```User``` access you can register (min 8 symbols for password, email must contain @), or use ```email``` - user@i.ua and ```password``` - user1234.<br />
For ```Admin``` access  use ```email``` - admin@i.ua and ```password``` - admin123.<br />

####All endpoints of my application (HTTP Method - url - permission):
```
POST: /register - all
GET: /cinema-halls - user/admin
POST: /cinema-halls - admin
GET: /movies - user/admin
POST: /movies - admin
GET: /movie-sessions/available - user/admin
GET: /movie-sessions/{id} - user/admin
POST: /movie-sessions - admin
PUT: /movie-sessions/{id} - admin
DELETE: /movie-sessions/{id} - admin
GET: /orders - user
POST: /orders/complete - user
PUT: /shopping-carts/movie-sessions - user
GET: /shopping-carts/by-user - user
GET: /users/by-email - admin
``` 