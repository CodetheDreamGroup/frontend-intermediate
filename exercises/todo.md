# Specification

## Customer Request

I would like a todo application to help me manage my work items throughout the week.

In order for it to be useful to me it needs to have several features that I am defining in this specification.

Once you have completed the development of the application, I will take ownership of the code so I will need detailed information on how to continue developing the application.

## Technical Requirements

I would like the application to be written using JavaScript, which I already have familiarity with, and to have a web UI using HTML and CSS.



## README

I would like an extensive README that documents what technology was used to build the application, as well as instructions on how to build it myself. 

Please include documentation on what data types were used for different portions of the application and why they were used, any details about testing the application, as well as the file/folder structure.


## Dependency Management

Please use [npm](https://npmjs.com) for package management. Specify your dependencies in a `package.json` file in the root directory of your app.

Please don't check the `node_modules` folder in to source control by using a `.gitignore`  file to avoid that.

## Functionality

### Viewing todos

There should be a way for me to view all of the current todos.

It should be possible to view all todos whether they are completed or not, as well as viewing only the uncompleted todos. By default when viewing the todos it should only show uncompleted todos.

It should also be possible to view an individual todo including its description and if it is completed or not.

If there are no todos at all, whether completed or not, then it should show a message saying "No todos created yet. Create one to get started."

If there are todos, but all of them are completed, then the default view of the todos should show/print a message saying 'Congratulations, you have completed all of your todos.'

After showing/printing the list of todos it should then show the a count of all of the todos show such as "12 uncompleted todos".

### Creating a new todo

There should be a way to create a new todo item. A todo item is very simple, it has a text description/title of the todo, as well as a value to represent if the todo is completed or not. When a new todo item is created it should not be marked as completed.

### Completing a todo

A todo should be able to be marked as completed.

### Editing a todo

There should be a way to change the description of a todo.

### Toggle all todos state

It should be possible to change the state of all of the todos to completed or not completed with a single action.

### Delete completed todos

There should be a way to delete all of the completed todos. This should remove them completely from the 

