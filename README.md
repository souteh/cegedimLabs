# cegedimLabs
JEST:

init Jest dependencies:

npm install –save-dev jest-cli babel-jest
npm install --save-dev  react-addons-test-utils
npm install --save-dev react-shallow-testutils	
to run Test: npm test




Isomrphoc:

1. install express and ejs: npm install --save express ejs react react-dom
2. install the latest Babel version with support for ES6 and JSX as well as its peer dependency (webpack), use 
npm install --save webpack babel-core babel-loader babel-preset-es2015 babel-preset-react
to run express server: babel-node server.js 




REdux:
url: https://codesandbox.io/s/github/reduxjs/redux/tree/master/examples/todos

State:

{
  visibilityFilter: 'SHOW_ALL',
  todos: [
    {
      text: 'Consider using Redux',
      completed: true
    },
    {
      text: 'Keep all state in a single tree',
      completed: false
    }
  ]
}



...............

Presentationnel components:
	TodoList is a list showing visible todos.
		todos: Array is an array of todo items with { id, text, completed } shape.
		onTodoClick(id: number) is a callback to invoke when a todo is clicked.

	Todo is a single todo item.
		text: string is the text to show.
		completed: boolean is whether the todo should appear crossed out.
		onClick() is a callback to invoke when the todo is clicked.

	Link is a link with a callback.
		onClick() is a callback to invoke when the link is clicked.

	Footer is where we let the user change currently visible todos.

	App is the root component that renders everything else.

Container component: subscribe to redux ... to connect prez component to redux
	VisibleTodoList filters the todos according to the current visibility filter and renders a TodoList
	FilterLink gets the current visibility filter and renders a Link.
		filter: string is the visibility filter it represents.
