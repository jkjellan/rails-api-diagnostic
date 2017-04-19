# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
// A backend persists data, and allows multiple remote clients to access a central resources.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The controller uses the model to fetch data
```

Which layer in the MVC pattern communicates with the model?

```md
The controller communicates with the model
```

Why don't we use views in our interpretation of the MVC pattern?

```md
We handle our views on the front-end.
```

What does C.R.U.D stand for?

```md
Create
Read
Update
Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
We define CRUD actions (i.e. methods) in the controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Index
Show
Create
Update
Destroy

--Not used:
New
Edit
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
-Router determines which controller should handle the request
-Controller determines which model to request data from
-Model determines how to retrieve data from the database
-Controller sends JSON to client.
-Client renders JSON.
```

What is the command to generate a new rails-api app?

```bash
rails new [app name]
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
rake db:drop
rake db:create
rake db:migrate
rake db:rollback
rake db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate scaffold Pet name:string age:integer
```
