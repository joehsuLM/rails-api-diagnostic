# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
To process requests and send them back to the client/front-end
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model layer is used by the controller ot fetch data
```

Which layer in the MVC pattern communicates with the model?

```md
The controller communicates with the model
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Accessing the Model directly from views does not separate concern and goes against the MVC pattern. 
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Model and Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
index, show, create, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1) User sends the GET request from a client or front-end app to get the contets of ID 1 from the peope URI.
2) The server receives the GET request and passes it to an API that handles data for people
3) The API parses the request using the appropriate controller
4) The data for ID 1 in the is retrieved from the people model.
5) The model passes the data back to the controller.
6) The controller sends the information back to the view layer which displays it in a readable/user-friendly format on the client/front-end.
```

What is the command to generate a new rails-api app?

```bash
rails generate
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
● db:drop
● db:create
● db:migrate
● db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate model pet name age
```
