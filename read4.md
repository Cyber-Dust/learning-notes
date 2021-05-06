# HTML
## Chapter 4: "Links"

The layout of writing a link in HTML

```
<a href="https address">NAME</a>
```

## USE `<a>` element for links

- Same Folder
```
<a href="folder.html">EXAMPLE</a>
```
- Child Folder
```
<a href="child/folder.html">EXAMPLE</a>
```
- Grandchild Folder
```
<a href="grandchild/child/folder.html">EXAMPLE</a>
```
- Parent Folder
```
<a href="../index.html">EXAMPLE</a>
```
- Grandparent Folder
```
<a href="../../.html">EXAMPLE</a>
```

## Chapter 15: "Layout"

Layout is one of the biggest aspects of building a webiste.

With layout, you can control flow and organize what the user sees, usually using `div` element.

- Browsers display pages in normal flow unless you specify relative, fixed positioning, or absolute.
  - *Relative* flow shits the placement of the element.
  - *Normal* flow is default behavior and stationary
  - *Absolute* positions the element in relation to its containing element.

- Pages can be fixed width or liquid layouts.

- CSS Frameworks are rules for common tasks

- Multiple CSS files can be inhected into HTML

Block-level elements: Start on a new line

Inline elements : flow in between surrounding text

# JAVASCRIPT

## Chapter 3 : “Functions, Methods, and Objects"

## FUNCITONS
A function lets you group together a series of statements to perform a task.
- Calling the function: When you ask it to perform its task.
```
sayHello();
```
- Parameters: pieces of info passed to a function.
- Return Value: the response from the funciton you wrote.

To declare a functon: 
- Use function keyword
- Give the function a name
- The statements that perform the task go in a code block.

ex.)
```
funciton sayHello() {
  document,write('Hello World');
}
```
When declaring funciton, use parameters `()`

## PAIR PROGRAMMING
Pair progrmming is: double headed programming uzing a driver and a navigator.

The driver is handling the mechanics of programming; whereas, the navigator will be using words to guide the driver.

Pair programming:
- Greater efficiency
- Engaged collaboration
- Learning from fellow students
- Improves social skills
- Job interview readiness
- Work enviornment readiness

Code Fellows utilizes pair programming.

[<==ReturnToHome](README.md)