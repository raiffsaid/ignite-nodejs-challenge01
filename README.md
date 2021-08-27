<<<<<<< HEAD
# Rocketseat Ignite Bootcamp - Challenges

## Node.js
### Chapter I
- [x] 1. Node.js concepts
- [ ] 2. Working with middlewares
- [ ] 3. Correcting the code

### Chapter II
- [ ] 1. Introduction to SOLID
- [ ] 2. Documenting with Swagger

### Chapter III
- [ ] 1. Database Queries
- [ ] 2. Database modeling

### Chapter IV
- [ ] 1. Unit testing
- [ ] 2. Integration testing

### Chapter V
- [ ] 1. Transfers with FinAPI

### Chapter VI
- [ ] 1. Building with serverless
=======
# Challenge 01 - Node.js concepts

## 💻️ About the challenge
### In this challenge, you must create an application to train what you've learned so far in Node.js!

### This will be an application to manage tasks (*todos*). You will be allowed to create a user with `name` and `username`, as well as to use CRUD of *todos* :
- Create a new *todo*;
- List all *todos*;
- Change the `title` and `deadline` of an existing *todo*;
- Mark a *todo* as done;
- Delete a *todo*;

All this for each specific user (the `username` will be passed in the header).

## ⚙️ Running the application locally

- Clone the repository:
```console
> git clone https://github.com/raiffsaid/ignite-nodejs-concepts.git
```

- Navigate to the root project directory
```console
> cd ignite-nodejs-concepts
```

- Install the dependencies using Yarn 
```console
yarn
```

- Run the test suit 
```console
yarn test
```

- Run the project 
```console
yarn dev
```

## 🗂️ Application resources
### You can use tools like [Insomnia](https://insomnia.rest/) or [Postman](https://www.postman.com/) for HTTP requests.
1. Create a new user: `http://localhost:3333/users` [POST]
    - The route must receive `name` and `username` inside the body request. When registering a
    new user, it must be stored inside an object in the following format:
```jsonc
{
	"id": "uuid",
	"name": "Danilo Vieira", 
	"username": "danilo", 
	"todos": []
}
```

2. List *todos* from a specific user: `http://localhost:3333/todos` [GET]
   - The resource must receive, through the request header, a `username` property containing the username of the user and return a list of all taks for that user.

3. Create a new *todo*: `http://localhost:3333/todos` [POST]
    - The resource must receive a `title` and `deadline` within the request body, and a `username` property containing the username of the user within the request header. Each task must be in the following format: 

```jsonc
{
	"id": "uuid", 
	"title": "Name of the task",
    "done": false, 
	"deadline": "2021-12-12T00:00:00.000Z", 
	"created_at": "2021-08-27T00:00:00.000Z"
}
```
4. Update a *todo*: `http://localhost:3333/todos/:id` [PUT]
    - The resource must receive, through the request header, a `username` property containing the username of the user and receive the `title` and `deadline` properties inside the body. It is only necessary to change the `title` and `deadline` of the task that has an `id` equal to the `id` present in the route parameters.

5. Update a *todo* property: `http://localhost:3333/todos/:id/done` [PATCH]
    - The resource must receive, by the request header, a `username` property containing the username of the user and change the `done` property to `true` in the *todo* that has an `id` equal to the `id` present in the route parameters.

6. Delete a *todo*: `http://localhost:3333/todos/:id` [DELETE]
    - The resource must receive, through the request header, a `username` property containing the username of the user and exclude the *todo* that has an `id` equal to the `id` present in the route parameters.

## 📝️ License

This project is under MIT license. Check the file [LICENSE](https://github.com/raiffsaid/ignite-nodejs-concepts/blob/main/LICENSE) for more details.

---

Made by <a href="https://www.linkedin.com/in/raiffsaid">Raiff Said</a>
>>>>>>> 64c1972a196b8a3e45739002b4cdd7ce65ab2775
