# ai-api-401

This is going to be the most kickass README EVER.
# LAB - 31&32?

## Custom Hooks: Sockets and Fetch

### Author: Ai

### Links and Resources
* [submission PR](http://xyz.com)
* [travis](http://xyz.com)
* [back-end](http://xyz.com) (when applicable)
* [front-end](http://xyz.com) (when applicable)

#### Documentation
* [api docs](http://xyz.com) (API servers)
* [jsdoc](http://xyz.com) (Server assignments)
* [styleguide](http://xyz.com) (React assignments)

### Modules
#### `form.js`  `q.js`  `shopping.js`  `todo.js`  `todo-list.js`
##### Exported Values and Methods
`form.js` exports useForm which is used by `todo` and `shopping` to create new items for either shopping  or chores. It saves form data to the server, updating the state, which will be picked up by the q-server. See next: 

`q.js` exports useQ which is used in the `todo-list.js` which is subscribed to our `todo.js ` form events. It publishes those events to the list for viewing. As events are submitted to the API server, the q serve is listening for it, and renders them into our list module, the `todo-list.js`.

###### `useState`
We use this in `form.js`

###### `useEffect`
You can see this in action in the `todo-list.js`

### Setup
#### `.env` requirements
* `PORT` - Port Number 3000
* `MONGODB_URI` - URL to the running mongo instance/db

#### Running the app
* `npm start`
* Endpoint: `/src/index.js/`
  * Returns our react application--`app.js`.
* Endpoint: `/src/app.js/`
  * Returns the actual applcation with modules.
  
#### Tests
* How do you run tests? --npm run test but no tests have yet been created!
* What assertions were made?
* What assertions need to be / should be made?

#### UML
Link to an image of the UML for your application and response to events