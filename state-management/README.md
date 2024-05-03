# ![Intro to React - State Management](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be introduced to the concept of state in React.

## State management

It is useful for a component to hold data that can change through time in response to events such as user actions. React uses ***state*** as the mechanism for this. Think of state as the present status or condition of something.

For example, a television has state - what its the volume set to, what channel or input is being shown, or whether it is on or off would all be considered state.

As a person using a television you can also manipulate that state - for example, by hitting the volume up button on the remote. When you do this, the television responds by increasing the volume and by displaying the new volume on the screen.

React components each have the capability to have state. That state can be changed in response to events - typically in response to a user action. This ability to change makes React components dynamic.

React enforces this concept by using state variables created with a special function built into React called a ***hook***. These state variables are unique, because when we want to modify them, we don't do so directly - they're instead updated using a ***setter function***.

![State example](./assets/state-example.png)
