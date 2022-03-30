# Add Event Listener

Using the browser console, attach an event listener of any type to [this page](http://www.republiquedesmangues.fr/). Be creative! Here is one example (click the mango after running this code):

```js
const mango = document.querySelector('#mangue');
mango.addEventListener('click', function (event) {
  mango.style.animation = 'spin'
  mango.style.animationDuration = '0.5s'
  mango.style.animationIterationCount = 'infinite'
  mango.style.animationTimingFunction = 'linear'
})
```


Here is my code:

```js
const mango = document.querySelector("#mangue")
let count = 0
mango.addEventListener("click", (event) => {
    count += 1
    if (count <= 1 && count > 0) {
        alert("MANGO")
    }
    if (count <= 2 && count > 1) {
        alert("Yep, still a mango")
    }
    if (count <= 3 && count > 2) {
        alert("This mango ain't going anywhere")
    }
    if (count <= 4 && count > 3) {
        alert("NO MANGO")
        mango.src = ""
    }
})
```
