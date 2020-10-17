# frontend-interviews-encyclo
Following are the list of interview questions on HTML5, CSS3, JS, ES6, ReactJS, Redux.<br/>

## HTML

<details>
    <summary style='font-weight:bold'>1. Why do we use data tags in HTML?</summary>
    <p>The `<data>` tag is used to add a machine-readable translation of a given content. This element provides both a machine-readable value for data processors, and a human readable value for rendering in a browser</p>
</details>

## CSS

<details>
    <summary>1. Create a google calendar</summary>
    <p>Implement using CSS grid and DOM manipulation</p>
</details>

## JS & ES6

<details>
    <summary>1. Write a polyfill for bind()</summary>
    <p><a href ='https://github.com/HebleV/100-days-of-code/blob/master/Wesbos_JS_tuts/polyfills/bind.js'>Polyfill for bind</a></p>
</details>

## ReactJS

<details>
    <summary>1. Explain the lifecycle methods of React</summary>
    <p>This can be little tricky as there are different answers for a class and a functional component. Perhaps, a better reply would be to ask if they are looking for a class component or a functional component. I believe certainly functional as it is the latest and most used. But it helps to know both the lifecycle methods.<br/>
    <a href='https://blog.logrocket.com/lifecycle-methods-with-the-useeffect-hook/'>Functional components</a>
    <a href='https://blog.logrocket.com/the-new-react-lifecycle-methods-in-plain-approachable-language-61a2105859f3/'>Class Components</a>
    <b>Note: </b> There is also an older version of lifecycle methods for the class components where certain lifecycle methods have become deprecated like ComponentWillMount and ComponentWillUpdate. 
    </p>
</details>

## Redux

<details>
    <summary>1. Explain the flow of Redux</summary>
    <p>We write an action which is dispatched when an event is triggered. This inturn calls the respective reducer which doesn't directly update the state but rather makes a copy and returns a new state and thus updating the store. This will rerender the component.
<b>Note:</b> Usually setState is not used or required when using redux. Based on the requirements it can be used. But mostly initial states and default props should be used. As local states are difficult to maintain
</p>
</details>
