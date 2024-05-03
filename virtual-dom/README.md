# ![Intro to React - Virtual DOM](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to describe how React uses a virtual DOM to make targeted updates to the UI.

## Virtual Document Object Model (virtual DOM)

Often, when state is changed what is shown to the user changes as well. React handles these UI updates through a mechanism called the ***virtual DOM***. The virtual DOM is a copy of the actual DOM  any updates that should be made to the actual DOM and acts as a staging area for changes that will eventually be implemented.

When React makes these changes, it does so  keep track of changes in the actual DOM by comparing it to the virtual DOM.

Here is a breakdown of the process:

- React renders an in-memory representation of the DOM, known as the **virtual DOM**.
- After the rendering, React compares the latest virtual DOM to the previous Virtual DOM and computes only the difference, known as the **diff**.
- React then updates the browser's actual DOM with the actual changes (the computed **diff**).

![Virtual DOM](./assets/virtual-dom.png)