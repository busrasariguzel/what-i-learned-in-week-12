# `What I Learned in Week 12`

### `Componentize`
* There are couple of different websites we can you to make our website pretty if we do not focus on the style. The websites are:
* [Materialize CSS](https://materializecss.com/)
* [Bootstrap](https://getbootstrap.com/)
* [Semantic UI](https://semantic-ui.com/)
* [Bulma](https://bulma.io/)
* These websites offer css style templates for other programmers to use. It is very useful and easy to use. * For my project, I used bootstrap. 
* Directions:
  1. You copy and paste the link to the head section on your html. There is also another link to copy as a script tag to the end of your body section.
  2. Then you copy different components and paste them to your html. I copied many different components such as nav bar and they looked very cool.

* Here is a snapshot of my project with bootstrap:

* ![image](component.png)
----


### `Object Oriented Programing`
``` Javascript
const Stack = function() {
  return {
    items : [],
    
    add : function(str){
      return this.items.push(str);
    },
    remove : function() {
      return this.items.pop();
    },
    peek : function() {
      return this.items[this.items.length -1]

    },
  }
}
```
---

### `TODOM`
* In this project, we practice event listener functions and created a to do list. 
* The challenge was to remove the text after clicking on it. The second to do project had the similar challenge. We were supposed to have line through after clicking it and removing them after clicking remove button. We,as a group, tried many times and spend time to overcome this challenge.
* Some code we used in this project :
``` javascript
const removeButton = document.querySelector('.remove-todo');
removeButton.onclick = removeFromList;
let newLi = document.querySelectorAll('li');
const clearCompleted = function (){
  for (let i = 0; i<newLi.length; i++){
    if (newLi[i].textDecoration ='line-through'){
        newLi[i].style.display= 'none'
    }
    }
}

document.querySelector('.clear-all').addEventListener('click', clearList)
document.querySelector('.remove-all-todo').addEventListener('click', clearCompleted)
```



