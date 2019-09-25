# ai-api-401

This is going to be the most kickass README EVER.
# LAB - 31&32?

## Custom Hooks: Sockets and Fetch

### Author: Ai

### Links and Resources
* [submission PR](https://github.com/401-advanced-javascript-aimurphy/ai-api-401/pull/3)
* [travis](http://xyz.com)
* [back-end](https://apm-tcp-mssngr.herokuapp.com) (this one isn't working ☹️)
* [front-end](https://ai-api-401.herokuapp.com/api/v1/todo) (when applicable)
* alternate [front/api](https://api-js401.herokuapp.com/api/v1/todo) and [back/q](https://q-js401.herokuapp.com)


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
We use this in `form.js` to work like `this.setState` in that we are using it to handle the event of adding to our lists and updating the list with the new submission fro mthe form.

###### `useEffect`
You can see this in action in the `todo-list.js` where it works like `componentDidMount`, this is the actualadding part--so the usestate updates and use effect is making sure you can see that.

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