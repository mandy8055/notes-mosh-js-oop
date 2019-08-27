# Constructors
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
    //console.log('this', this);
    this.radius = radius;
    this.draw = function() {
        console.log('draw');
    }
    //return this; // return auto when user 'new' keyword
}
const another = new Circle(1);

```
---
#### new keyword
1. create an empty object `{}`
2. set this point to that object
3. return that object to the function (`Circle()`)