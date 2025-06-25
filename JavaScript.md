# Grammar

1. ## Variables and Constants
```javascript
let age = 30;
age = 28; // 'let' declares a changeable variable
const name = "Jack"; // 'const' declares a constant, which cannot be changed
```
2. ## Type of Data
```javascript
const number = 10; // number
const string = "Hello"; // string
const boolean = true; // boolean
const nullValue = null; // null
const undefinedValue = undefined; // undefined
```
**Basically, we can define a constant using any word,but to keep code clear, we should follow naming rules.**

3. ## operator

| operator  | descript     | example          | result |
|-----------|--------------|------------------|--------|
| +         | add          | 10+5             | 15     |
| -         | subtraction  | 10-5             | 5      |
| *         |multiplication| 10*5             | 50     |
| /         | division     | 10/5             | 2      |
| %         | remainder    | 10%5             | 0      |
| ++        | increment    | let x = 10; x++; | 11     |
| --        | decrement    | let x = 10; x--; | 9      |
| &&        | AND          | true && false    | false  |
| \|\|      | OR           | true \|\| false  | true   |
| !         | NOT          | !true            | false  |

4. ## if
```JavaScript
const score = 85;
if (score >= 90) {
  console.log("Excellent");
} else if (score >= 80) {
  console.log("Good");
} else if (score >= 70) {
  console.log("OK");
} else {
  console.log("Substand");
}//result:Good
```

5. ## For
```JavaScript
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

6. ## Functions
```JavaScript
function add(a, b) {
  return a + b;
}

const result = add(3, 4);
console.log(result); // 7
```
7. ## Objects and Arrow Functions
**Objects**
```JavaScript
const person ={
  name:"Jack",
  age:28,
  address:{
      city:"Tokyo",
      phoneName:"000-0000-0000"
  },
  hobbies:["Reading","Traveling"]
};

console.log(person.name); // Jack
console.log(person["age"]); // 28
console.log(person.address.city); // Tokyo
console.log(person.hobbies[0]); // Reading
```
**Arrow Functions**
```JavaScript
const name = "Tiger"; // Standalone Variable
const obj = {
  name: "Cat",// Variable
  sayHi: function () {
    const inner = () => {
      console.log("this.name:", this.name);
      console.log("name:", name);
    };
    inner();
  },
};
obj.sayHi();
// this.name: Cat 
// name: Tiger  
```
**`this.name` refers to the property `name` on the object that `this` points to (in this case, `obj`), so it outputs "Cat".  
`name` without `this` refers to a variable in the outer (higher) scope, which here is the global variable `name = "Tiger"`.  
If the object does not have a `name` property, then `this.name` will be `undefined`, because `this` points to the object but that property doesn't exist.  
Note that standalone variables like `name` are not related to the object's properties and are resolved based on scope, not `this`.**

8. ## DOM
**Select and Print**
```HTML
<div id="app">
  <h1>Title</h1>
  <p class="message">morning！</p>
</div>
```
```JavaScript
//selection componment
const title = document.getElementById("app").querySelector("h1");
const message = document.querySelector(".message");
//print content
console.log(title.textContent); // Title
console.log(message.textContent); // morning！
```
**Add**
```HTML
<ul id="list">
  <li>item1</li>
  <li>item2</li>
</ul>
```
```JavaScript
const list = document.getElementById("list");

const newItem = document.createElement("li");
newItem.textContent = "newItem";

list.appendChild(newItem);
```
**Event Listener**
```HTML
<button id="btn">click</button>
```
```JavaScript
const button = document.getElementById("btn");
button.addEventListener("click", () => {
   title.textContent = "You clicked the button!";
});
```
