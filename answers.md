# Answers:

## JS:
1 Promise is asynchrounious operation with some methods that do task one after another to run the given task.But, Callback is a child function that gets called after parent function is called.

2 Event Bubbling: 
  * when an event happens on HTML element and by default event goes from that element to the top, to it's parent element, and it's parent element to it's parent and so on.
  
 Event Delegation: 
 * when that event being delegated on the way of bubbling to it's parent element.
 
 Event Capturing: 
 * catching an event coming from the parent element to it's child element.
 

3 call(forComa, coma), apply([array]) methods, you can write a method that can be used on different objects.
  bind() creates a new function that will have "this"-(currentObject) set to the first parameter passed to bind().
  

4 Class Inheritance: instances inherit from classes (blueprint), and create sub-class relationships(Parent -> Child). Instances are typically instantiated via constructor functions with the `new` keyword.
Code example:
```javascript
class Father{
  constructor(name, age){
    this.name = name;
    this.age = age;
  }
  introduce(){
    console.log("My name is", this.name);
  }
}

var kanat = new Father("Kanat", 29);
kanat;
kanat.introduce();

//============== inheritance starts here

class Son extends Father {
  constructor(name, age, has){
    super(name, age);
    this.has = has;
  }
  property(){
    console.log("I have a", this.has);
  }
}
var tima = new Son("Tima", 25, "computer");
tima;
tima.introduce();
tima.property();
```

Prototypal Inheritance: instances inherit directly from other objects. Instances are typically instantiated via factory functions or `Object.create()`.
Code example:
```javascript
function Father(eyes, skin){
  this.eyes = eyes;
  this.skin = skin;
}
Father.prototype.can = function(){//method for Father
  console.log("Can bring food");
}
 //instance     object
var kanat = new Father("brown");//instanstiating object
kanat;
kanat.can();

//========================  inheritance starts here

Son.prototype = Object.create(Father.prototype);//ES6 extends Father
function Son(){
  Father.call(this, "blue", "black");//ES6 super()
}
var bala = new Son();
bala.can();


```

## CSS:
1 CSS gradients let you display smooth transitions between two or more specified colors

2 A tooltip is often used to specify extra information about something when the user moves the mouse pointer over an element

3 I'm currently looking for this answer )) ...sorry guys

4 3-ways to apply: inline, internal, external

5 In the "head"- because when browser brings HTML to user CSS codes get imported first before 'body'.

6 If 2 or more CSS selectors apply to the same HTML element, the one with higher specificity wins out. Specificity order(1-Important,2-inline, 3-class, 4-element

7 position values are:
  * static(by default is static)
  * fixed(doesn't move even when you scroll)
  * absolute(the same as fixed but respects scrolling)
  * relative(checks parent--doesn't take properties `left-right` to set positions)
  * sticky(positioned based on user scroll)


## HTML
 1 Inline elements are: ISLAB(img,span,link,a,button).The rest elements are block elements.
 
 2 Scalable Vector Graphics: used for designing logos etc. Defines the graphics in XML format using mathematical relation.
 
 3 Self closing tags are: BILI(br,img,link,input)
 
 4 Semantic HTML--brought meanings for elements naming(nav,header,aside,footer,article etc..), also self closing tags and now they don't have to be closed with "/" slash, such as (`<img /> <img>`).
 
 5 Some characters are reserved in HTML in order to use them we use entities...such as "<" -> "&lt;"

## General:
 1 React(for mobile: React Native), Angular(for mobile: Ionic), Vue etc.
 
 2 
   * use sprite(minimize assets)
   * use adaptive images,
   * evaluate plugins(making sure cdn-s are up to date and minified)
   * reduce http calls,
   * use cdn(for location services),
   * review hosting package(if package plan is not loaded)
   * enable HTTP keep-alive response headers,
   * configure expires headers
 
 3 
   * reset CSS(resetting default CSS to new such as {margin: 0} etc..),
   * normalize CSS(small CSS file that aims to make built-in browsers styling consistent across multiple browsers)
   * use frameworks(bootstrap, reactstrap)
   * cross browser testing( testing manually and find standard ground for every browser)

4 Unit testing tools are: Jasmine, Ava, Tape, Mocha, 

5 Task Runners are: Gulp, Grunt.In one word automation. Doing such as converting Less to CSS and minifying JS files etc..

6 
* React(JS library but with Redux, Router it goes as a framework, uses JSX syntax. React is good for small apps and large apps)-by Facebook
 * Angular(framework that uses Typescript scripting laguage that is similar to JS, all core features are included which is good for large apps but bad for small apps)-by Google
 * Vue(uses JS syntax in well-known way and keeps HTMl and JS, CSS seperate from each other in one file, manages layouts with components, learning curve is easy)-by developers
 
 7 You can use Firefox or Chrome to debug but i prefer Chrome and it's inspector:
  * read the error and use `console.log()` to log out the error
  * use breakpoints: `step over`, `step in`, `step out`
  * use `debugger` statement in your source code
  * use developer tools to make debugging easier such as `react dev tools` that is in chrome web store 
  
 8 Single page app:
  * reduces HTTP calls
  * does not require page reloading during use, front end files run in the browser--it is fast 
  * SPA requests the markup and data independently and renders pages straight in the browser
    
  * first time loading is slow because it gives to user all front end source codes at once
  * if user disables javascript in their local browser then app is not gonna be presentable of it's own way
  * not an easy task to make SEO optimization of a Single-Page Application

Multi-page app:
  * very good and easy for proper SEO management. It gives better chances to rank for different keywords since an application can be optimized for one keyword per page.
  * to get from one page to another requires page reloading, essentially it makes a request to a server
  * to display a new page to user first request gets sent to server to bring new page, so it is slow
  * frontend and backend development are tightly coupled
  
 9 Asynchrnous Javascript and XMl. Essentially it's an operation that does something without reloading the web page. Before in web development all developers used to use XMl format but, now every modern developer uses JSON. People still calling it AJAX--rather then AJAJ(Asynchronous Javascript and Json) 
 
 10 End-to-end testing is a Software testing methodology to test an application flow from start to end.
 
 11 Web accessibility means that websites, tools, and technologies are designed and developed so that people with disabilities can use them.
 
 12 Browser API is simply is an API, provided by the browser and that we can communicate with using JavaScript. Such as an extension of the HTML <iframe> element that allows web apps to implement browsers or browser-like applications.
