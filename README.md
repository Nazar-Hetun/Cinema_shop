# Cinema Shop
This project shows the work of a cinema store, where users have a shopping cart and can add tickets to it and place an order.
Admin can add new cinema halls, movies, do CRUD operations with movie sessions.
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

### All endpoints of my application (HTTP Method - url - permission):
```
-Register new User.
POST: /register - all 

-Get all cinema halls.
GET: /cinema-halls - user/admin
-Add new cinema hall.
POST: /cinema-halls - admin

-Get all movies.
GET: /movies - user/admin
-Add new movie.
POST: /movies - admin

-Get all avaiable movie sessions for selected time.
GET: /movie-sessions/available - user/admin
-Get movie session by id.
GET: /movie-sessions/{id} - user/admin
-Add new movie session.
POST: /movie-sessions - admin
-Update movie session.
PUT: /movie-sessions/{id} - admin
-Delete movie session.
DELETE: /movie-sessions/{id} - admin

-Show all User orders.
GET: /orders - user
-Complete order.
POST: /orders/complete - user

-Add movie session to cart.
PUT: /shopping-carts/movie-sessions - user
-Get User shopping cart.
GET: /shopping-carts/by-user - user

-Get User by his email.
GET: /users/by-email - admin

``` 
