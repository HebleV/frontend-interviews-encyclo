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

## JS & ES6

<details>
    <summary>1. Write a polyfill for bind()</summary>
    <p><a href ='https://github.com/HebleV/100-days-of-code/blob/master/Wesbos_JS_tuts/polyfills/bind.js'>Polyfill for bind</a></p>
</details>

<details>
    <summary>2. In a promise chain of 5 promises, what if promise 4 fails will next promise be executed ?</summary>
    <p>No, it does not execute next</p>
</details

<details>
    <summary>3. Write a polyfill for Promise</summary>
    <p>Implement using setTimeout</p>
</details

<details>
    <summary>4. What is the difference between Promise.race() and Promise.all()?</summary>
    <p>This returns a promise as soon as any one of the Promise is resolved where as in Promise.all(), it waits until all the promises are resolved.</p>
</details

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

## Redux

<details>
    <summary>1. Explain the flow of Redux</summary>
    <p>We write an action which is dispatched when an event is triggered. This inturn calls the respective reducer which doesn't directly update the state but rather makes a copy and returns a new state and thus updating the store. This will rerender the component.<br/>
<b>Note:</b> Usually setState is not used or required when using redux. Based on the requirements it can be used. But mostly initial states and default props should be used. As local states are difficult to maintain
</p>
</details>
