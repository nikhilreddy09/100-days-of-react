# 100-days-of-react
This repository is dedicated to 100 days of react challenge where ill be posting updates each and every day

I am starting with Learn React Js by freecodecamp.org on Youtube on my first day of react.


<h1>Day 1</h1>
1. I have started to learn ReactDOM and JSX.<br>
2. Functional Components.<br>
3. Parent child Components.<br>

<p>We can use ReactDom to render the required content. we need to import react-dom before we can start using it </p>
<code>import ReactDom from 'react-dom'</code>
we can use this statement in the file where we want to render the data.
<code>ReactDom.render("Data to be rendered" , document.getElementById("root")</code>

<p>we can have html elements as the first argument and the second argument serves as the place where the react needs to be rendered in the html page. Here we selected root id.</p>

<h4>Functional Components</h4>
<p> functional components are nothing but the seperate functions that are passed to ReactDom to render.</p>
<p>For example if we have a function such as </p>
<code> function App() {
 //data to be rendered
    }
  </code>
  <p>We can use this in the ReactDom render as follows :</p>
  <code> ReactDom.render( "Name", document.getElementById("root")</code>
  <p>We substitue the name as ("'<'App'/>'") in the above method to render the App function. remove the inverted commas.</p>
  
  <h4>Parent child components</h4>
  <p>Parent child components is something similar to functional components where inside the App function we have several small child components which render a specific task. for example having header , nav , footer inside the app function so that its easy to findout which function is rendering which element.</p>
  
  <p>if we are defining the function in another file we need to export those function by using.</p>
  <code> export default "Function name"</code>
  <p>and then import the function in the file we are using it by using import statement as follows.</p>
  <code> import Name from "path"</code>
  
  <p>We can style the files in react by using css. we need to import the CSS file by using the import statement as follows . suppose the css file name is App.css then :</p>
  <code>
 import './App.css'
</code>
<p>I have started creating a react application called to-do-list, <a href="https://github.com/nikhilreddy09/to-do-list">Click here for repo.</a> </p>
