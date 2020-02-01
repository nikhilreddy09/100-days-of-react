# 100-days-of-react
This repository is dedicated to 100 days of react challenge where ill be posting updates each and every day

I am starting with Learn React Js by freecodecamp.org on Youtube on my first day of react.

<p>I have started creating a react application called to-do-list, <a href="https://github.com/nikhilreddy09/to-do-list">Click here for repo.</a> </p>


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

<h1>Day 2</h1>
1. props <br>
<p>Inorder to get javascript into JSX file we use curly braces around it "{ }" . for example if we want to access a variable named age inside our jsx we do the following inside the opening and closing tags.
 <code> <Tagopen>my age is {age} </tagclose></code>
 <p>Props in react are used to send data to the function that we want to render on our screen . we can send props in form of javascript object . </p>
 <code>  
contact = {{name : "Nikhil" , phone : "1234567890" , email : "n@gmail.com"}} 
</code> . 
<p>We can send this object to the tag that it refers to and it is stored inside of props</p>
<code>
 function tag(props) {
   console.log(props.contact.name)
 }
</code>
<p>In this way we can send data to the function using props and sending it in the form of objects.</p>
<p>Here i have created a simple application to see how we can work with props in react : https://github.com/nikhilreddy09/props-react</p>
<h1>Day 3</h1>
<p>Today i have been learning about mapping components. </p>
<p>I have included a small project on how mapping components work here : https://github.com/nikhilreddy09/mapping-components-react</p>
<h1>Day 4</h1>
<p>Today i have started learning about class components.</p>
<p> We can use the class components by extending the class which we want to create with React.Component so that we can use some of the properties from Component.</p>
<p>We need to put everything we want to render inside render function within class component for example :</p>
<code>
 class ToDoItem extends React.Component {
     
    render() {
      return (
        <div className="todo-item">
            <input type="checkbox" checked={this.props.completed} />
          <p>{this.props.text}</p>
        </div>
        )
    }
}

</code>

<p>Here we have created a class ToDoItem which extends React.Component and then used a render function to render the data within.</p>
<p>In order to access props within class componnet we do that by using this.props.name to get the prop with key as name</p>
