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
