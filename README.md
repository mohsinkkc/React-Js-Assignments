React Js Assignments
Mohmad mohasin
1) What is JavaScript Output method?
ans.
⦁	document.write(): It is mostly used for testing purposes or for inserting dynamic 
⦁	content into a web page.
⦁	console.log(): This method is used to output data to the console of the browser's 
⦁	developer tools
⦁	window.alert(): This method is used to display a message in a dialog box.
⦁	innerHTML: It is commonly used to dynamically update the content of a web page.
2)How to used JavaScript Output method?
ans.
⦁	This will output "Hello World!" to the console of the browser's developer tools.
<script>
console.log("Hello World!");
⦁	This will output "Hello World!" directly onto the web page
document.write("Hello World!"); 
This will output "Hello World!" inside the <p> element with the id attribute of  "output".

document.getElementById("output").innerHTML = "Hello World!"; 
⦁	This will display a dialog box with the message "Hello World!".
window.alert("Hello World!");

</script>
3) How to used JavaScript Events to do all examples?
ans.
1) This will display output "Hello World!" directly onto the web page when the button is 
clicked
 <button id="outputButton">Click me!</button>
<script>
document.getElementById("outputButton").addEventListener("click", function() {
document.write("Hello World!");
});
</script> 

 2)This will display output "Hello World!" to the console of the browser's developer tools 
when the button is clicked
<button id="outputButton">Click me!</button>
<script>
document.getElementById("outputButton").addEventListener("click", 
function() {
console.log("Hello World!");
});
</script> 
. 
 3) This will display a dialog box when the button is clicked

<button id="outputButton">Click me!</button>
<script>
document.getElementById("outputButton").addEventListener("click", 
function() {
window.alert("Hello World!");
});
</script> 
 4) This will output "Hello World!" inside the <p> element when the button is 
clicked.

<button id="outputButton">Click me!</button>
<p id="output"></p>
<script>
document.getElementById("outputButton").addEventListener("click", 
function() {
document.getElementById("output").innerHTML = "Hello 
World!";
});
</script> 
MODULE-3

1) What is React Js?
ans.
React is a JavaScript library.
It was developed by Facebook and has gained a lot of popularity in recent years 
due to its performance, flexibility, and reusability.
React allows developers to create reusable UI components that can be easily 
combined to create complex and interactive interfaces
It uses a virtual DOM (Document Object Model) to efficiently update the UI 
without the need for full page reloads.
2). What is NPM in React Js?
ans.
When a developer starts a new React project using Create React App, NPM is used 
to install all the necessary packages and libraries required to get the project up 
and running.
3). What is Role of Node Js in react Js?
ans.
Node.js is a server-side JavaScript runtime environment, which means it allows 
JavaScript code to run on the server-side rather than just in the browser.
In the context of React.js, Node.js is often used as a development tool for building 
and testing React applications. 
Developers can use npm to install React and other third-party packages required 
for building a React application.
4). What is CLI command In React Js?
ans.
. In React.js, CLI (Command Line Interface) commands are used to perform various 
tasks related to building, testing, and deploying React applications.
Some common CLI commands used in React.js development include:
npx create-react-app my-app:
This command creates a new React application called "my-app" using the Create 
React App tool.
npm start:
This command starts the development server and opens the application in the 
default browser. It also automatically reloads the application when changes are 
made.
5). What is Header and Content Components in React Js?
ans.
Header and Content components are common types of components used in 
React.js applications to define the layout and structure of the user interface.
Overall, the Header and Content components are simple examples of how 
components can be used to build the layout and structure of a React.js 
application.
6). What is Components in React Js?
ans.
Components are the building blocks of React.js applications. In React.js, a 
component is a self-contained piece of code that defines the UI of a portion of the 
application. Components can be thought of as reusable templates for creating UI 
elements such as buttons, forms, or navigation menus.
components are classes that extend the React.Component class and define a 
render() method that returns a UI element.
Overall, components are a fundamental concept in React.js and are essential for 
building modular, reusable, and maintainable user interfaces.
7) How to install React Js on Windows, Linux Operating System? How to install NPM and How to check 
version of NPM.
Ans.
Download and install Node.js from the official website:
https://nodejs.org/en/download/
Open a terminal or command prompt.
Run the following command to install ReactJS globally:
npm install -g create-react-app
Once the installation is complete, you can create a new React project by running the following 
command:
create-react-app my-app-> my-app is project name
start the development server:
npm start
8). How to check version of React Js.
ans.
node -v
9). How to change in components of React Js?
ans.
Locate the component you want to make changes to. Components are usually located in the 
src/components directory in a typical ReactJS project.
Open the file containing the component code in your preferred code editor.
Make the necessary changes to the component code. 
Save the changes to the file.
If the changes you made affect the appearance of the component, refresh the browser window where 
the application is running to see the changes.
10). Create Increment decrement state change by button click.
ans.
import React, { useState } from "react";
function Increment() {
 const [number, setNumber] = useState(0);
 const Increment = () => {
 setNumber(number + 1);
 };
 const Decrement = () => { // Define function to handle increment button click
 setNumber(number - 1);
 };
 return (
 <div>
 <button onClick={Increment}>+</button> 
 <h1>{number}</h1>
 <button onClick={Decrement}>-</button>
 </div>
 );
}
export default Increment;
