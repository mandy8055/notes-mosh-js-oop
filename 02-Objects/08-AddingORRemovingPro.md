# Adding or Removing Properties

## Cases where bracket notations are used instead of dot notation
- `propertyName` is dynamic i.e. not known in advance and we need to set the value of that property. See **example for point 1**.
- `propertyName` is an invalid identifier. See **example for point 2**.

## Adding

```js
function Circle(radius) {
  this.radius = radius;
  this.draw = function() {
    console.log('draw');
  };
}

const circle = new Circle(10);

circle.location = { x: 1 };

const propertyName = 'center-location'; // example for point 2
const propertyName = 'center location'; // example for point 2
//circle.center-location;
//circle.center location;

circle[propertyName] = { x: 1 }; // example for point 1
```

## Removing

```js

delete circle['location'];
        // OR
delete circle.location;
```
