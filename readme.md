What is Middleware?

=> Middleware is software which lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.

What is middleware in Web API?

=> Middleware are software components that are assembled into an application pipeline to handle requests and responses. Each component chooses whether to pass the request on to the next component in the pipeline, and can perform certain actions before and after the next component is invoked in the pipeline.

What is middleware in backend?

=> Middleware is referred to as middle tier. Essentially Middleware links the front and back end of the system together acting as a bridge between the front and back end. It is often referred to as the glue between the data and the UI. The Middleware is therefore often where the business logic resides.

What is middleware in node JS?

=> Middleware functions are functions that have access to the request object ( req ), the response object ( res ), and the next middleware function in the application's request-response cycle. The next middleware function is commonly denoted by a variable named next.
```js
const express = require('express')
const app = express()

const myLogger = function (req, res, next) {
  console.log('LOGGED')
  next()
}

app.use(myLogger)

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(3000)
```

How many types of middleware in Node JS?

=> There are five different types of middleware: 3rd Party, Router, Application, Error-handling, and Built-in.