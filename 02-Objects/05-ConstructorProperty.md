# Constructor
```javascript
// Factory Function
function createCircle(radius) {
    return {
        radius,
        draw: function() {
            console.log('draw');
        }
    };
}

const circle = createCircle(1);

// Constructor Function
function Circle(radius) {
    this.radius = radius;
    this.draw = function() {
        console.log('draw');
    }
}
const another = new Circle(1);

```

#### Constructor function
- `another.constructor` return `Circle functon` factory function

#### Built-in constructor function
- `circle.constructor` return `f Object() { [native code] }` 

---

#### Constructor 
```javascript
let x = {} // object literal
// let x = new Object();

// Built-in    |   Literals 
new String();   // '', "", ``      String literls
new Boolean();  // true, false     Boolean literals
new Number();   // 1, 2, 3  ...    Number literals

```