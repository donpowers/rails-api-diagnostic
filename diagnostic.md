# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
The backend's role is to persist data used by you application.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The model is used to fetch data.
```

Which layer in the MVC pattern communicates with the model?

```md
The controller communicates with the model
```

Why don't we use views in our interpretation of the MVC pattern?

```md
The view is the UI interface.  We use the MVC pattern using curl type request
to simulate what the UI would send us.
```

What does C.R.U.D stand for?

```md
Creat Read Update Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Model
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Index, Show Create Update, Destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
The routes.rb is look at to see if there is an action that supports the request.
The route then calls the GET(show) metod in the people controller.
The controller will then execute the methods that will send the 'find' command to the DB
The model(DB) will respond to the controller
The controller will look at the response and determine success/failure and send a response.
```

What is the command to generate a new rails-api app?

```bash
rails generate controller Greetings Hello
```

What is the command to start an instance of a rails server?

```bash
$ bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
rake db:drop
rake db:create
rake db:migrate
rake db:seed db/seed.rb
rake db:setup does db:create, db:schema:load, db:seed

```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold Pet name:string age:integer
```
