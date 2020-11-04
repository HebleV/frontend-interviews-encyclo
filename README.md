# frontend-interviews-encyclo

Following are the list of interview questions on HTML5, CSS3, JS, ES6, ReactJS, Redux.<br/>

### HTML

<details>
    <summary style='font-weight:bold'>1. Why do we use data tags in HTML?</summary>
    <p>The <data> tag is used to add a machine-readable translation of a given content. This element provides both a machine-readable value for data processors, and a human readable value for rendering in a browser</p>
</details>

<details>
    <summary>2. What are the new features in HTML?</summary>
    <p><a href='https://www.w3schools.com/tags/tag_details.asp'>Details Tag</a></p>
</details>

## CSS

<details>
    <summary>1. Create a google calendar</summary>
    <p>Implement using CSS grid and DOM manipulation</p>
</details>

<details>
    <summary>2. What is difference between position fixed and absolute ?</summary>
    <p>Fixed means, the position of an element is fixed wrt the window like fixed header and absolute is element is independent of window and can be placed anywhere by using top, bottom, left, and right values</p>
</details>

<details>
    <summary>3. What is difference between position fixed and absolute ?</summary>
    <p>Fixed means, the position of an element is fixed wrt the window like fixed header and absolute is element is independent of window and can be placed anywhere by using top, bottom, left, and right values</p>
</details>

<details>
    <summary>4. What is position sticky ?</summary>
    <p>It behaves like relative position until it hits a certain offset value after which it behaves like position fixed.</p>
</details>

<details>
    <summary>5. What is CSS selector specificity ?</summary>
    <p>If there are two or more conflicting CSS rules that point to the same element, the browser follows some rules to determine which one is most specific and therefore wins out. The priority order of specificity is inline style, id, classes/attributes/pseudo classes, elements/pseudo elements 
</p>
</details>

<details>
    <summary>6. What is flex basis ?</summary>
    <p>Its the initial size or the width of the flex item</p>
</details>

<details>
    <summary>7. What is rem and em value in CSS ?</summary>
    <p>rem(Root em) - Relative to font-size of the root element
em - Relative to the font-size of the element (2em means 2 times the size of the current font)
</p>
</details>

<details>
    <summary>8. What is box model ?</summary>
    <p><a href='https://www.w3schools.com/css/css_boxmodel.asp'>More Details</a></p>
</details>

<details>
    <summary>9. What is :is() and :where() in CSS ?</summary>
    <p>is() pseudoclass is to reduce the repetition in selectors lists.
:where() pseudoclass is to keep the specificity of selector low
<a href='https://webplatform.news/issues/2020-06-04'>More Details</a></p>
</details>

<details>
    <summary>10. How do you achieve grid and flex layout using plain CSS ?</summary>
    <p>Updating...</a></p>
</details>

## JS & ES6

<details>
    <summary>1. Write a polyfill for bind()</summary>
    <p><a href ='https://github.com/HebleV/100-days-of-code/blob/master/Wesbos_JS_tuts/polyfills/bind.js'>Polyfill for bind</a></p>
</details>

<details>
    <summary>2. In a promise chain of 5 promises, what if promise 4 fails will next promise be executed ?</summary>
    <p>No, it does not execute next</p>
</details>

<details>
    <summary>3. Write a polyfill for Promise</summary>
    <p>Implement using setTimeout</p>
</details>

<details>
    <summary>4. What is the difference between Promise.race() and Promise.all()?</summary>
    <p>This returns a promise as soon as any one of the Promise is resolved where as in Promise.all(), it waits until all the promises are resolved.</p>
</details>

<details>
    <summary>5. What is wrong in below code?</summary>
    <p>```this.setState((prevState, props) => {
 return {
   streak: prevState.streak + props.count
 }
})
 ```<br/>
 <b>Answer:</b> Nothing is wrong with it. It’s rarely used and not well known, but you can also pass a function to setState that receives the previous state and props and returns a new state, just as we’re doing above. And not only is nothing wrong with it, but it’s also actively recommended if you’re setting state based on the previous state.
 </p>
</details>

<details>
    <summary>6. What will be the output here in func()?</summary>
    <p>```const test = {
    comp: ’IT World',
    role: 'dev',
    func: () => {
        return `In ${this.comp}, I am a ${this.role}`
    }
}
 ```<br/>
 <b>Answer:</b>this.comp and this.role will be undefined.<br/>
 But if you change above code from arrow function to normal function i.e. 
```const test = {
   comp: 'IT World',
   role: 'dev',
   func: function() {
       return `In ${this.comp} i am a ${this.role} .`
   }
}``` <br/>
<b>Answer:</b>this.comp and this.role will be IT World and dev respectively.
 </p>
</details>

<details>
    <summary>7. How do we achieve inheritance before ES6 ?</summary>
    <p>Update...</p>
</details>

<details>
    <summary>8. How do we make sure that certain property only not to be updated in an object ?</summary>
    <p>Using object.preventExtensions();</p>
</details>

<details>
    <summary>9. Javascript is synchronous or asynchronous ?</summary>
    <p>Synchronous and single threaded<a href='https://medium.com/better-programming/is-javascript-synchronous-or-asynchronous-what-the-hell-is-a-promise-7aa9dd8f3bfb#:~:text=under%20the%20hood.-,JavaScript%20is%20Synchronous,in%20progress%20at%20a%20time.'>Good read</a></p>
</details>

<details>
    <summary>10. What are the new features in ES6, 7,8… ?</summary>
    <p><a href='https://medium.com/@madasamy/javascript-brief-history-and-ecmascript-es6-es7-es8-features-673973394df4'>New features</a></p>
</details>

<details>
    <summary>11. What would console print ?</summary>
    <p>```console.log(a);
Var a = 7;```</p>
<b>Answer:</b> Undefined coz Values are hoisted only when declared not when initialized.
But if it is let or const then it will be ReferenceError.
</details>

<details>
    <summary>12. What is the difference between a normal function and arrow function ?</summary>
    <p><a href='https://dmitripavlutin.com/differences-between-arrow-and-regular-functions/'>More details</a>
</details>

<details>
    <summary>13. What is the purpose of call and apply ?</summary>
    <p><b>Answer:</b> If you know how many arguments you would be passing then use call and if you are not sure how many arguments you would be passing or if the arguments are already an array or an object then use apply.
</details>

<details>
    <summary>14. What is 5 > 4 > 3 ? </summary>
    <p><b>Answer:</b>False coz JS coerces 5>4 first which is true (1) then true(1) > 3 = false;</p>
</details>

<details>
    <summary>15. What is 3 + true ?</summary>
    <p><b>Answer:</b>4 coz JS coerces true to 1 and 3 + false would be 3.</p>
</details>

<details>
    <summary>16. Different ways to create object in javascript ?</summary>
    <p>Updating...</p>
</details>

<details>
    <summary>17. Find the longest subarray having sum equal to s ?</summary>
    <p><b>Answer:</b><a href='https://codepen.io/HebleV/pen/QWybGaV?editors=1012'>Solution</a></p>
</details>

<details>
    <summary>18. Merge the keys and values to form an object?</summary>
    <p><b>Answer:</b><a href='https://codepen.io/HebleV/pen/zYrGoYb?editors=1112'>Solution</a></p>
</details>

<details>
    <summary>15. What is 3 + true ?</summary>
    <p><b>Answer:</b>4 coz JS coerces true to 1 and 3 + false would be 3.</p>
</details>

<details>
    <summary>16. What is functional chaining ?</summary>
    <p><b>Answer:</b>Updating...</p>
</details>

<details>
    <summary>17. How do you create inheritance in JS ?</summary>
    <p><b>Answer:</b>Updating...</p>
</details>

<details>
    <summary>18. What is the purpose of deep cloning ?</summary>
    <p><b>Answer:</b>To create a deep copy or new object independent from old one. One way is first json.stringify the object or array and json parse it. Another way is, It is created using lodash. Object.assign creates a shallow copy means the new object will still have same old references - <a href="https://flaviocopes.com/how-to-clone-javascript-object/#:~:text=Deep%20copy%20vs%20Shallow%20copy,-A%20shallow%20copy&text=If%20an%20object%20references%20other,independent%20from%20the%20old%20one">More info</a></p>
</details>

<details>
    <summary>19. What are static methods ?</summary>
    <p><b>Answer:</b>Static methods are often utility functions, such as functions to create or clone objects, whereas static properties are useful for caches, fixed-configuration, or any other data you don't need to be replicated across instances. Usually, static methods are used to implement functions that belong to the class, but not to any particular object of it.</p>
</details>

<details>
    <summary>20. What is a singleton ?</summary>
    <p><b>Answer:</b>It is an object which can be instantiated only once. So even if you repeatedly call its constructor same instance is returned</p> <a href='https://www.dofactory.com/javascript/singleton-design-pattern'>More info</a>
</details>

<details>
    <summary>21. What is the difference between map, filter, and reduce ?</summary>
    <p><b>Answer:</b>Updating...</p>
</details>

<details>
    <summary>22. What sort method will you use for building web app ?</summary>
    <p><b>Answer:</b>Updating...</p>
</details>

<details>
    <summary>23. How will you make sure your app is not crashed if there are no values or null in nested json objects ?</summary>
    <p><b>Answer:</b>We can make use of new JS feature of optional chaining operator `?.`</p><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining'README.md>More info</a>
</details>

<details>
    <summary>24. How will you find the type of an element or object ?</summary>
    <p><b>Answer:</b>Using typeof</p>
</details>

<details>
    <summary>25. What is {} + [] = ?</summary>
    <p><b>Answer:</b>0 because of the type of conversion which is empty object and empty array.</p>
</details>

<details>
    <summary>26. What are the type of object and array ?</summary>
    <p><b>Answer:</b>typeof object = object; <br/>
		   typeof array = object;</p>
</details>

<details>
    <summary>27. What is the difference between slice and splice ?</summary>
    <p><b>Answer:</b>Slice doesn’t change existing array but splice does.</p>
</details>

<details>
    <summary>28. What are higher order functions or components ?</summary>
    <p><b>Answer:</b>The functions that can take other functions as inputs or provide functions as its output. Ex : map, filter, reduce </p>
</details>

<details>
    <summary>29. What are the differences between local, session storages and cookies ?</summary>
    <p><b>Answer:</b>            		 local 		      session              cookies
	Capacity     		 10 mb                  5mb	          4kb
		Expiry	        		 Never                  on tab close         manually set
		Storage location	browser	     browser                browser n server

	          Methods
		localStorage
          localStorage.setItem(‘name’, john);
          localStorage.getItem(‘name’);
          localStorage.removeItem(‘name’);
         Similar methods for session storage.

	Cookies
         Document.cookie = ‘name=john; expires =’ + new Date(9999, 0 ,1).toUTCString();
</p>
</details>

<details>
    <summary>30. What is the output ?</summary>
    <p><b>Question:</b>a();
b();
c();
function a() {
   console.log(1)
}
 
var b = function() {
   console.log(2);
}
 
var c = () => {
   console.log(3);
}
</p>
<p>Answer: 1<br>
                Error : b is not a function<br>

            Note: It will not even go to c() call coz of error at b(); but c() will also throw same error.</p>
</details>

<details>
    <summary>31. Write a program for function sum(1)(2)(3) which gives output as 6 ?</summary>
    <p><b>Answer:</b>let sum = function(a) {
		                return function(b) {
			                return function(c) {
                                    return a + b + c;
                                   }
                             }
                    }
</p>
</details>

<details>
    <summary>32. What are generators and how will you know if it is an iterator ?</summary>
    <p><b>Answer:</b>You can know if it is an iterator if function is preceded by * symbol.</p>
</details>

<details>
    <summary>33. What are the differences between arrow function and normal function ?</summary>
    <p><a href="https://dmitripavlutin.com/differences-between-arrow-and-regular-functions/">More info</a></p>
</details>

<details>
    <summary>34. How do you achieve inheritance ?</summary>
    <p><b>Answer:</b>Updating...</p>
</details>

<details>
    <summary>35. What is function currying ?</summary>
    <p><a href="https://www.youtube.com/watch?v=vQcCNpuaJO8&ab_channel=AkshaySaini">More info</a></p>
</details>

<details>
    <summary>36. What are map and weakmap ?</summary>
    <p>Map doesn’t allow to garbage collect the object reference and WeakMap does allow. 
Map accepts objects, strings, num etc but WeakMap accepts only objects as keys.
Map has size property but WeakMap does not have.
</p>
</details>

<details>
    <summary>37. What is “2” + “2” - “2” ?</summary>
    <p><b>Answer:</b>20 - Because + will concatenate which will give 22 and - will type coerce and convert it into numbers. So 22 - 2 = 20</p>
</details>

<details>
    <summary>38. What is typeof null ?</summary>
    <p><b>Answer:</b>Object</p>
</details>

<details>
    <summary>39. What is the output 
console.log(a,b)
{
let a = 10;
var b = 20
console.log(a,b)
}
console.log(a,b)
</summary>
    <p><b>Answer:</b>Reference Error : a is not defined.</p>
</details>

<details>
    <summary>40. What is the value of following ?</summary>
    <p><b>Answer:</b> 0 === false; // false <br>
              0 == false // true
</p>
</details>

<details>
    <summary>41. What are generators ?</summary>
    <p><b>Answer:</b>Generators are basically the functions which returns the generator object which holds the entire generator iterable that can be iterated using the next() method. 
I has yield key word which is like return keyword. 
next() method will return an object with “done” flag and “value” key. 
</p>
</details>

<details>
    <summary>42. Why does const allow change in values when assigned to an object ?</summary>
    <p>Because it refers to a memory address not the actual object itself.
</p>
</details>

<details>
    <summary>43. What are primitive data types and reference data types ?</summary>
    <p>Primitive : Number, Boolean, String, Undefined, Null
Reference : Functions, Array and objects (though typeof of all are object only)
For primitive, Can assign a value directly.
For reference, you cannot coz you assign to an address in a memory not actual value.<a href='https://codeburst.io/explaining-value-vs-reference-in-javascript-647a975e12a0#:~:text=Assigning%20by%20Reference,var%20reference%20%3D%20%5B1%5D%3B'>More info</a></p>
</details>

<details>
    <summary>44. What is the difference between object.preventExtensions, seal and freeze methods ?</summary>
    <p>These deals with adding, deleting, and modification of properties.
preventExtensions => Doesn’t allow addition of new properties.
Seal => Doesn’t allow addition of new properties and deletion of existing   properties.
Freeze => Doesn’t allow addition, deletion and modification of object properties.</p>
</details>

<details>
    <summary>45. What is the output for below destructuring assignment ?</summary>
    <p>1-  const foo = ['one', 'two', 'three']; 
   const [red, yellow, green] = foo; 
   console.log(red); // "one" 
   console.log(yellow); // "two" 
   console.log(green); // "three"
    </p>
    <p>2- When deconstructing an object, if a property is not accessed in itself, it will continue to look up along the prototype chain.
    let obj = {self: '123'}; 
    obj.__proto__.prot = '456';
    const {self, prot} = obj; 
    // self "123"
    // prot "456"（Access to the prototype chain）
    </p>
    <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment'>More info</a>
</details>

<details>
    <summary>46. Convert the nested array into single dimension array ?</summary>
    <p>Input : let arr = [1,[2,3,[4,5,[6,7]]]];
       Output: arr=[1,2,3,4,5,6,7]
    </p>
</details>

<details>
    <summary>47. What are rest and spread operators ?</summary>
    <p>Updating...</p>
</details>

<details>
    <summary>48. Reverse a string and print it</summary>
    <p><a href='https://github.com/HebleV/100-days-of-code/blob/master/Wesbos_JS_tuts/reverse.js'>Check here</a></p>
</details>

<details>
    <summary>49. How does generators work in backend or make it iterable ?</summary>
    <p>Updating...</p>
</details>

<details>
    <summary>50. What is the difference between null and undefined ?</summary>
    <a href='https://codeburst.io/javascript-whats-the-difference-between-null-undefined-37793b5bfce6'>Read here</a>
</details>

<details>
    <summary>51. How to ensure that only one of the object properties is not writable or readable ?</summary>
    <p>This is achieved using Object.defineProperty.
	Let name = {
		firstname: “john”
		}
        Object.defineProperty(name, ‘lastName’,{
		value : “doe”,
		writable:false
} )
Now you can update firstname but not lastname.
</p>
</details>

<details>
    <summary>52. What would be the output in below code ?</summary>
    <a href='https://wesbos.com/for-of-es6'>Read here</a>
</details>

<details>
    <summary>53. What is the output ?</summary>
    <p>Let x = function(){
	return
	{
	 message:’hi’
	}
}
x();
</p>
<p>Answer: x is undefined coz in a function after return statement there must be braces rather than on next line else JS will insert a comma and return.</p>
</details>

<details>
    <summary>54. What is the value of console.log(Math.max()) ?</summary>
    <p>infinity coz that is the lowest number in maths when no input is given.</p>
</details>

<details>
    <summary>55.What is the output ?</summary>
    <p>const array = [1, 2, 3, 4, 5];
console.log("a")
array.forEach((el, i) => {
    console.log(el);
});</p>
<p>Answer: 
console.log("b")
// a 1 2 3 4 5 b
Because forEach is synchronous even though it takes a callback function.</p>
</details>


<details>
    <summary>56.What is the output [...[...'...']].length ?</summary>
    <p>Answer: 3</p>
</details>

## ReactJS

<details>
    <summary>1. Explain the lifecycle methods of React</summary>
    <p>This can be little tricky as there are different answers for a class and a functional component. Perhaps, a better reply would be to ask if they are looking for a class component or a functional component. I believe certainly functional as it is the latest and most used. But it helps to know both the lifecycle methods.<br/>
    <a href='https://blog.logrocket.com/lifecycle-methods-with-the-useeffect-hook/'>Functional components</a><br/>
    <a href='https://blog.logrocket.com/the-new-react-lifecycle-methods-in-plain-approachable-language-61a2105859f3/'>Class Components</a><br/>
    <b>Note: </b> There is also an older version of lifecycle methods for the class components where certain lifecycle methods have become deprecated like ComponentWillMount and ComponentWillUpdate. 
    </p>
</details>

<details>
    <summary>2. How can you handle error boundary ?</summary>
    <p><a href='https://kentcdodds.com/blog/use-react-error-boundary-to-handle-errors-in-react'>React Error Boundary</a></p>
</details>

<details>
    <summary>3. Why React recommends to use keys in map ?</summary>
    <p>Because React internally keeps track of items if it has changed.</br><a href='https://kentcdodds.com/blog/understanding-reacts-key-prop'>More details</a></p>
</details>

<details>
    <summary>4. What is the disadvantage of using index for keys in map in React?</summary>
    <p>Because React cannot differentiate if the element was removed or just content is changed. So it will just compare every other DOM element.<a href='https://medium.com/@vraa/why-using-an-index-as-key-in-react-is-probably-a-bad-idea-7543de68b17c'>Good read</a></p>
</details>

<details>
    <summary>5. How do you display a default 404 error page in react JS ?</summary>
    <p>Using the Redirect method from react-router-dom <br/>
    ```<Route component={ErrorPage} />```
    </p>
</details>

<details>
    <summary>6. What are the new features added in React 16.7 ?</summary>
    <p>React Hooks, React.memo, React.lazy, React.suspense, Context, error boundary, and React.Fragment.
    </p>
</details>

<details>
    <summary>7. What is useCallback</summary>
    <p>If there is a function(lambda function) which is re-rendered everytime then we can use useCallback to prevent it. <a href='https://www.youtube.com/watch?v=-Ls48dd-vJE'>More</a></p>
</details>

<details>
    <summary>8. What is virtual DOM?</summary>
    <p>Updating...</p>
</details>

<details>
    <summary>9. What is shadow DOM?</summary>
    <p>Shadow DOM API helps in encapsulation of certain hidden elements from the actual DOM nodes/elements so that the hidden code doesn’t clash with actual DOM code. Shadow DOM api provides a way to attach a separate hidden DOM to an element (Shadow Host) of the actual DOM.  Example: HTML <video> tag
To attach a shadow dom, we use attachShadow method.
Example: let shadow = element.attachShadow({ mode: ‘open’});
In this element is the shadow host and shadow is the shadow root.
    <a href='https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM'>More Details</a>
</p>
</details>

<details>
    <summary>10. How can you improve performance of React app ?</summary>
    <p>Updating...</p>
</details>

<details>
    <summary>11. What is getDerivedStateFromError() in ErrorBoundary component ?</summary>
    <p>It is used to render a fallback UI after an error is thrown.</p>
</details>

<details>
    <summary>12. What is componentDidCatch() in ErrorBoundary component ?</summary>
    <p>It is used to log error information.</p>
</details>

<details>
    <summary>13. What is React Context ?</summary>
    <p> It provides a way to pass data through the component tree without having to pass props down manually at every level. For ex: we have a parent component with some data. And it has child and grand child components. In the current scenario if we want to pass data then we will have to pass data to child then grandchild. Even though child doesn’t need data but still we are passing data. So using context we can now directly pass data from parent to grand child.
It uses React.Provider which provides data and React.Consumer which accesses/consumes data.
</p>
</details>

<details>
    <summary>14.How can we access DOM in React ? Can we access ?</summary>
    <p>Using Refs which are created by React.creatRef(). These Refs are created and attached to React elements via the ref attribute.</p>
</details>

<details>
    <summary>15. What is one way and two way bindings ?</summary>
    <p>one way data binding -> model is the single source of truth . whatever happens on UI triggers a message to model to update a part of data. So data flows in single direction and which becomes easy to understand.
two way data binding -> any change in UI field updates the model and any change in model updates the UI field.
</p>
</details>

<details>
    <summary>16. How do you render React on server side ?</summary>
    <p>Updating...</p>
</details>

<details>
    <summary>17. What is getDerviedStateFromProps in React lifecycle ?</summary>
    <p>This is the place where the state object is set based on initial props.
This method can be invoked in both mounting and updating phases.
</p>
</details>

<details>
    <summary>18. What is reconciliation in React ?</summary>
    <p>The process of finding the minimum number of changes that must be made in order to make virtual DOM and actual DOM tree identical. So keys play an important role in reconciliation. <a href='https://www.youtube.com/watch?v=b8IcYOV5_Rc'>More info</a></p>
</details>

<details>
    <summary>19. Is setState an asynchronous or synchronous ?</summary>
    <p>Asynchronous - Because it makes a call to callback function <a href='https://medium.com/@wereHamster/beware-react-setstate-is-asynchronous-ce87ef1a9cf3'>More info</a></p>
</details>

<details>
    <summary>20. What happens if we declare setState inside render () ?</summary>
    <p>It will be an infinite loop</p>
</details>

<details>
    <summary>21. What is the difference between componentWillReceiveProps and componentDidUpdate?</summary>
    <p>componentWillReceiveProps gets called before the rendering begins. It compares incoming props to current props and decide what to render.</p><br/>
    <p>componentDidUpdate gets called after any rendered HTML has finished loading. It receives 2 arguments prevProps & prevState.</p>
</details>

<details>
    <summary>22. How will you declare setTimeout in React component ?</summary>
    <p>It can be declared in useEffect and then return the clearTimeout() to unmount the component.</p>
</details>

<details>
    <summary>23. What is the purpose of super in constructor ?</summary>
    <p>To bind this to parent class component</p>
</details>

<details>
    <summary>24. What is the advantage of using arrow functions in React components ?</summary>
    <p>It will bind this to surrounding code context or to function so this will avoid bugs.</p>
</details>

<details>
    <summary>25. What is code splitting ?</summary>
    <p>It is splitting your code in such a way that, only that part of code is loaded required for the current screen. You can achieve this using dynamic imports (webpack) and lazy loading react components. ( Webpack will asynchronously load the components or spits out different files for different components. ) For 3rd party libraries or vendor files, it will load for first time and cached for ever in browser, so that it doesn’t load again when user visits for second time.</p>
    <a href='https://www.youtube.com/watch?v=bb6RCrDaxhw'>More info</a>
</details>

<details>
    <summary>26. How do you measure performance of React components or application ?</summary>
    <p>1.Use React profiler to see what components are taking lot of time to load<br>
	  2. Use perf library.<br>
  3. Use useMemo/React.Memo hooks to cache a component
</p>
</details>

<details>
    <summary>27. What is memoization ?</summary>
    <p>Memoization is the idea of caching a value so that you don’t have to compute every single time. </p>
</details>

<details>
    <summary>28. What does useMemo/React.Memo do ?</summary>
    <p>If you are sure that a function always returns the same computed value for a given input then there is no need to recompute or recalculate the value every single time. The value can be cached. This is done using useMemo or React.Memo.</p>
</details>

<details>
    <summary>29. What are the disadvantages of using useMemo ?</summary>
    <p>One has to use useMemo judiciously and efficiently because if you use useMemo for functions which are not required to be memoized then it uses a lot of memory overhead and causes performance issues again.</p>
</details>

<details>
    <summary>30. What is useRef ?</summary>
    <p>It is like useState but it doesn’t render every time there is an update. It holds the data or persists data/update between different renders without re-rendering the component.</p>
</details>

<details>
    <summary>31. Write a 2 line code to increment count by 5 using useState ?</summary>
    <p>const [count, setCount] = useState(0);
              setCount(count + 5);
</p>
</details>

<details>
    <summary>32. What are the advantages of using functional components over class components in React ?</summary>
    <p>
    <ul>
    <li>You don't have to manually bind "this" like in class component</li>
    <li>Simple and easy to test</li>
    </ul>
    </p>
</details>

<details>
    <summary>33. How can you compare previous state and previous props in react hooks ?</summary>
    <p>By writing a custom hook using the useRef <a href="https://blog.logrocket.com/how-to-get-previous-props-state-with-react-hooks/">More info</a></p>
</details>

<details>
    <summary>34. How do you manage state now in React using hooks ?</summary>
    <p>It is like useState but it doesn’t render every time there is an update. It holds the data or persists data/update between different renders without re-rendering the component.</p>
</details>

<details>
    <summary>35. What are performance metrics that you will check for a web app ?</summary>
    <p>
        <ul>
            <li>Loading Time</li>
            <li>Network Requests</li>
            <li>Caching</li>
            <li>Code Splitting</li>
        </ul>
    </p>
</details>

<details>
    <summary>36. How can you ensure a component or a thing is not re-rendered in class and functional component ?</summary>
    <p>Updating...</p>
</details>

<details>
    <summary>37. What is a lambda function in React ?</summary>
    <p>Everytime the component is rendered, the function is recreated.</p>
</details>

<details>
    <summary>38. What is useRef ?</summary>
    <ul>
        <li>Stores a previous value</li>
        <li>Helps in persisting the state between different renders without actually re-rendering the component. In contrast useState re-renders everytime.</li>
    </ul>
</details>


## Redux

<details>
    <summary>1. Explain the flow of Redux</summary>
    <p>We write an action which is dispatched when an event is triggered. This inturn calls the respective reducer which doesn't directly update the state but rather makes a copy and returns a new state and thus updating the store. This will rerender the component.<br/>
<b>Note:</b> Usually setState is not used or required when using redux. Based on the requirements it can be used. But mostly initial states and default props should be used. As local states are difficult to maintain
</p>
</details>

<details>
    <summary>2. Does reducer update data?</summary>
    <p>Yes it does but it doesn’t directly update state object but rather return a new updated object</p>
</details>

<details>
    <summary>3. How will you update/render a table list of data using react and redux ?</summary>
    <p>write one more component only for table body which will render table body given a table data. It will loop through data and render those lists.</p>
</details>

<details>
    <summary>4. How do you update data in react-redux app ?</summary>
    <p>Based on requirement we dispatch appropriate actions which can fetch api data and call to another action with type and payload or directly we dispatch action with type and data which has been sent to reducer.
Note: Usually setState is not used or required when using redux. Based on the requirements it can be used. But mostly initial states and default props should be used. As local states are difficult to maintain
</p>
</details>


## PWA

<details>
    <summary>1. What is a service worker ?</summary>
    <ul>
        <li> Runs in the background of users browser.</li>
        <li>Acts like a proxy server between app, browser and network.</li>
        <li>Allows apps to continue working offline in case of loss of internet</li>
        <li>Efficient caching of assets and make them available when user device is offline</li>
        <li>They run on a *separate thread *from the main JavaScript code of our page, and don't have any access to the DOM structure. This introduces a different approach from traditional web programming — the API is non-blocking, and can send and receive communication between different contexts. You are able to give a Service Worker something to work on, and receive the result whenever it is ready using a Promise-based approach.</li>
    </ul>
</details>

<details>
    <summary>2. What is manifest.json in PWA ?</summary>
    <p>It is a json file containing info about app like title, logi link, splash screen, background n theme color etc. It makes the website installable.</p>
</details>

<details>
    <summary>3. How do you make a website installable ?</summary>
    <ul>
        <li>A web manifest with all fields</li>
        <li>Website is served from a secure https connection</li>
        <li>An icon to represent the app on device</li>
        <li>Service worker registered to make work offline</li>
    </ul>
</details>

<details>
    <summary>4. How do you store data offline in PWA ?</summary>
    <ul>
        <li>Using cacheAPI which is part of service workers</li> 
        <li>Use indexedDB with a promise wrapper</li>
    </ul>
</details>

<details>
    <summary>5. Explain the service worker lifecycle ?</summary>
    <ul>
        <li>The install event is the first event a service worker gets, and it only happens once.</li>
        <li>A promise passed to installEvent.waitUntil() signals the duration and success or failure of your install.</li>
        <li>A service worker won't receive events like fetch and push until it successfully finishes installing and becomes "active".</li>
        <li>By default, a page's fetches won't go through a service worker unless the page request itself went through a service worker. So you'll need to refresh the page to see the effects of the service worker.</li>
        <li>clients.claim() can override this default, and take control of non-controlled pages.</li>
        <li>Install => Wait => active => Receive fetch and push events</li>
    </ul>
</details>

<details>
    <summary>6. What will the service worker script file have ?</summary>
        <ul>
            <li>It will have a cache-name i.e. app name</li>
            <li>URLs to cache</li>
            <li>Then add 3 event listeners to install ,fetch and activate.</li>
        </ul>
</details>

<details>
    <summary>7. How can you convert a create-react-app into a PWA ?</summary>
    <ul>
        <li>Include the above step 6q</li>
        <li>Update index.html to check if client browser supports service workers by adding another event</li> 
        <li>listener “load” the service worker</li>
        <li>Change serviceworker.unregister to serviceworker.register()</li>
        <li>Add progressive enhancement principle i.e. add some html content to display default html ...loading</li>
        <li>Add splash icon and update manifest.json</li>
        <a href='https://medium.com/@toricpope/transform-a-react-app-into-a-progressive-web-app-pwa-dea336bd96e6'>More info</a>
    </ul>
</details>

<details>
    <summary>8. How will you implement Server Side Rendering or SSR?</summary>
    <p>The reactjs provides the server-side rendering using 'react-dom/server' module.This module have renderToString() method to replace HTML string into the body as a response.</p>
        <ul>
            <li>Create a server file where you import express and provide port number</li>
            <li>Read the index.html from /build folder using fs.readfile (nodejs)</li>
            <li>On success, replace the HTML string i.e. <div id=’root’></div>imported app component with <div id=’root’>${ReactDOMServer.renderToString(<App/>)}</div></li>
            <li>In the react index.html file, replace React.render with React.hydrate</li>
            <li>Serve the static files from build folder</li>
            <li>Then add changes in server folder to ignore node modules and  add babel preset to compile</li>
            <li>Add ssr command in package.json in react app to run</li>
            <a href='https://www.youtube.com/watch?v=NwyQONeqRXA'>More info</a>
        </ul>
</details>
