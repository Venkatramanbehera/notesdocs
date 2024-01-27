# Important Interview Questions (ReactJS)

## How does react know what changes to make to the UI ?
Ans :- 
->React has this concept of a virtual DOM . This is a light weight representation of the real DOM, that can be changed
quickly when the code you write is proposing changes to UI.
->when the virtual DOM's tree is changed , react uses an algorithm called **'reconciler'** to compare the virtual DOM to real DOM.
->This algorithm is called as React Fiber(React v16+).

## How React Fiber work ?
Ans :-
-> Create a list of all changes to be rendered in the UI .
-> Schedules these changes to take place in the next phase.
-> Fiber then tells the DOM to render the changes using linked list traversal .

## What is the difference between re-rendering and mounting/unmounting ?
Ans :-
-> mounting/unmounting is creating and destroying the component instance.
-> re-rendering is executing component/function again .