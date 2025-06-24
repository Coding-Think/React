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
| --        | decrement    | let x = 10; x++; | 9      |
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

6. 

 


