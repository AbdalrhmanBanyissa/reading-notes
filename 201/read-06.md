# Problem Domain, Objects, and the DOM

## Problem domain

A problem domain is the area of expertise or application that needs to be examined to solve a problem. A problem domain is simply looking at only the topics of an individual's interest, and excluding everything else. For example, when developing a system to measure good practice in medicine, carpet drawings at hospitals would not be included in the problem domain. In this example, the domain refers to relevant topics solely within the delimited area of interest: medicine. This points to a limitation of an overly specific, or overly bounded, problem domain. An individual may think they are interested in medicine and not interior design, but a better solution exists outside of the problem domain as it was initially conceived. For example, when IDEO researchers noticed that patients in hospitals spent a huge amount of time staring at acoustic ceiling tiles, which "became a symbol of the overall ambiance: a mix of boredom and anxiety from feeling lost, uninformed, and out of control."

## Objects

![JS objects](https://miro.medium.com/max/875/1*AxAm_RRyMUsHvHUglQw2zw.jpeg)

Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

## Definition Examples

` var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"}; `

```javascript
var person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```

## DOM

> With the HTML DOM, JavaScript can access and change all the elements of an HTML document.

As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.

## html body  

![html body](/gallery/body.jpg)

## DOM tree  

![html body](/gallery/tree.jpg)
