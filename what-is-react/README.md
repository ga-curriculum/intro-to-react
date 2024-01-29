# ![Intro to React - What is React?](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

## What is React?

Origins and Development: Briefly touch on React's history and its development by Facebook. Highlight its initial purpose and how it has evolved.

Core Concept: Explain that React is a JavaScript library for building user interfaces, primarily for single-page applications. Emphasize its component-based architecture.

Usage and Popularity: Discuss its widespread use in the industry and its community support.







# Intro to React

## What is React?

- An open-source JavaScript library for building User Interfaces.
- It was open-sourced in May of 2013.
- Created by Jordan Walke, a Facebook engineer.
- Initially used to implement Facebook’s newsfeed in 2011 and in Instagram in 2012.
- Now being used by companies such as Netflix, Imgur, Airbnb, Walmart, and many more.
- A separate library, React Native, can be used to develop native iOS and Android mobile apps.

## When To Use React?

React is the go to front-end library when developing highly dynamic user interfaces.

## Why Use React?

React is the hottest front-end library around for building SPA user interfaces.

Adoption = Jobs !!!

## Modern JavaScript

The first thing to take note in the starting React app is that modern JavaScript is being used.

For example, note the use of `import` at the top of **`main.jsx`**. Just like we saw in our Unit 2 apps!

As React developers, we will be using newer features of JavaScript such as the **spread operator**, **destructuring assignment**, etc.


## Key Takeaways

At this point, the takeaway should be that:

- React apps consist of **components** that we code using JavaScript (and a special syntax known as JSX). You will not be creating any *.html files when developing a React app.
- The line of code that causes all of the components to be rendered for the first time is:
    
    ```jsx
    ReactDOM.createRoot(document.getElementById('root')).render(
      <React.StrictMode>
        <App />
      </React.StrictMode>
    );
    ```
    
- Rendering a React component, i.e., `<App>`, results in its nested components being rendered as well! Let that soak in for a bit.

## Try it Out and Make a Change

Now that you know a little bit about React components, try making some changes to the JSX within the `<App>` component and see how your changes are updated in the view.

Later today, we’ll be defining lots of our own components but first let’s look closer at some of the key concepts of React…

# Key Concepts of React

Let’s briefly review some key concepts of React. We’ll dig deeper in future lessons.

## Components

!https://i.imgur.com/TGZKfoI.png

- A React app’s UI consists of **components**.
- In React, we build an app’s UI by composing built-in and user-defined components.
- React’s built-in components are often referred to as React Elements. These are used to display actual DOM elements like `<div>`, `<h1>`, etc.
- The custom components we code are going to be used a lot like HTML tags. For example, in the diagram above, the UI is being built with tags like `<HomePage>`, `<SearchBar>`, `<EmployeeList>`, etc.
- Ultimately, our React components must contain React Elements if we want anything to appear on the page.
- React Elements can be styled using CSS and are the components that we will add event listeners to for responding to user interaction.
- Components that create the UI are created using 100% JavaScript. There is no HTML markup in React components, just something that looks like it…

## JSX

- Although a React component’s UI is ultimately defined by JavaScript, there is a better way to define the UI using a special syntax known as **JSX**.
- The syntax is an XML-based syntax that looks like HTML - as it should since HTML is also based on XML.
- Since our browsers do not understand JSX, it must first be transpiled (converted) into pure JS.

## State and Props

- Like most applications, a React component may have **state** (data/information).
- State can only be changed by the component that owns that state.
- When a component’s state is changed, that **entire** component is re-rendered, including all of its child components.
- A stateful component passes any state needed by child components as **props**.
- Props are accessible as key/value pairs on a **props** object. This props object is passed to the component every time it is rendered.
- **Props** in a component are always read-only.

## Rendering

Consider that most **state** is held at or near the top of the component hierarchy. Further, you now know that a component, and all of its children are re-rendered if **any** state changes.

Yeah, rendering happens frequently in a React app (whenever state changes), but thanks to React’s ingenious design, it’s very fast and efficient because of a mechanism known as the Virtual Dom. 

<aside>
📚 The Virtual DOM is a representation of the actual DOM and is a staging area for changes that will eventually be implemented. Because of that, React can keep track of changes in the actual DOM by comparing different instances of the Virtual DOM.

</aside>

- First, React renders to an in-memory representation of the DOM, known as the **Virtual DOM**.
- After the rendering is done, React compares the latest Virtual DOM to the previous Virtual DOM and computes only the difference, known as the **diff**.
- React then updates the browser’s actual DOM with the actual changes (the computed **diff**).
    
    ![Graphic from [Learning React Native](https://www.oreilly.com/library/view/learning-react-native/9781491929049/)](https://i.imgur.com/RmHCcDu.png)
    
    Graphic from [Learning React Native](https://www.oreilly.com/library/view/learning-react-native/9781491929049/)
    

## Review Questions ❓

1. **The User Interface in a React app is built using c____________s.**
2. **When ________ changes in a component, that component, and all of its children components are rendered.**