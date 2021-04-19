**React** 

- a user interface (UI) library created by Facebook. It helps you build interactive web applications made up of components.
- fast, modular, scalable, flexible, and popular

**Components** 
- Goodbye fixed templates, hello components

- Components are reusable chunks of content and behavior that can be put on a web page. A component is responsible for one job, which often involves rendering HTML.

- Should I write my component as a function or as a class? The general rule of thumb is if the component will not have a state, write it as a plain JavaScript function. If the component will have a state, write it as a class.

**JSX** 
- A special syntax for writing React code. JSX gets turned into regular JavaScript code by a compiler (i.e. Babel working in conjunction with Webpack).
- HTML elements can be written as JSX: 
    
    ```
    const panda = <img src='images/panda.jpg' alt='panda' width='500px' height='500px' />;
    ```
- JSX expressions can have exactly ONE outermost element, such as the below `<div>` If you have more than one outermost element, your code will break.
    ```
    const paragraphs = (
        <div id="outermostElement">
            <p>I am a paragraph.</p>
            <p>I, too, am a paragraph.</p>
        </div>
    );
    ```
- Another example, this time with JSX elements stored as an object:
    ```
    const myTeam = {
        center: <li>Benzo Walli</li>,
        powerForward: <li>Rasha Loa</li>,
        smallForward: <li>Tayshaun Dasmoto</li>,
        shootingGuard: <li>Colmar Cumberbatch</li>,
        pointGuard: <li>Femi Billon</li>
    };
    ```

- JSX elements can be either HTML-like, or component instances. JSX uses capitalization to distinguish between the two. That is the React-specific reason why component class names must begin with capital letters. In a JSX element, that capitalized first letter says, "I will be a component instance and not an HTML tag." So when naming a component, `<MyComponent />` is correct, but `<myComponent />` is incorrect.

**Methodology**

- A web page is laid out as a tree of nested components.  
- Components can contain other components (and native elements like divs and buttons).
- Components can be passed data to display.
- React has one-way data flow, meaning data is passed down from a component to its children, not the reverse. 

**Yarn:** 
- From now on when developing in React, only use yarn (instead of npm)

**Layouts**

    npm install -g yarn

(should be the same for mac & windows)
   
    yarn create react-app app_name
    
    cd app_name
    
    yarn start


- Before we wipe out the default contents of App.js & App.css, let's look them over
- Compare & contrast what's in these files to what we've been doing with main.js

- index.js write "Hello, World!" function
- in our JSX, inline HTML **class** becomes **className**, and **click** becomes **onClick** 
- component name must start with capital letter
- Add React Devtools extension to [Firefox](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/) or [Chrome](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi/related?hl=en)

**Tic-Tac-Toe Layout with React**
- Code-along

**AirBnB Layout with React**
- on your own, use React to remake the AirBnB layout
![AirBnB layout image]
https://raw.githubusercontent.com/SEI-SEA-1-25/css-airbnb/main/solution.jpg
