
## . What is a Design Pattern

Design **pattern stands for a programming concept that solves conceptual problems. It can be related to creating new objects, making the code more independent or modular, or even splitting your project into different layers of responsibility

<aside>
💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**

</aside>

## 2. What is MVC & how does it work

MVC design pattern introduces another abstraction layer that will help with the software planning, and also allow new programmers to navigate even in a bigger codebase. By splitting the thinking process into data, interface, and decisions, developers can reduce the number of source files that must be searched in order to add or fix functionality.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7845cbe7-9a0c-4367-8b43-5240850c159d/Untitled.png)

This design pattern separates code into three layers as the name suggests. 

- Model
    - job: stores game map, player and NPC data, game settings. Everything data.
    - is not aware of what Views or Controllers are looking at it.
    - can post and listen for events.
- View
    - job: draws on screen what the model represents.
    - is strongly aware of the model and its values.
    - can post and listen for events.
- Controller
    - job: taking keyboard and mouse input and posts matching events.
    - is strongly aware of the model and its values.
    - can post and listen for events.
- Events
    - job: coordinates messages between listeners.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6c7fbfda-6031-4bdd-a50a-1fed9ce80a67/Untitled.png)

This shows that even if the Controller does not know anything about the player's health, what level we are on, it still only catches key presses and sends out events to match.

Nor does the View care how the player is controlling our game. The View only cares about showing on screen the current model state. Since the View also listens to posted events, it will pick up mouse clicks and key presses that integrate into its widgets.

<aside>
💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**

</aside>

## 3. Problems that MVC is solving

Without structure, your code can get messy very easily and look like “spaghetti code”. To avoid this, developers should separate the game logic from the display code

The MVC pattern helps you break up the frontend and backend code into separate components. Allows multiple game developers need to update, modify, or debug a full-blown application simulta
