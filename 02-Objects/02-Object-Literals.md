# Object Literals
```javascript
const circle = {
    radius: 1,
    location: {
        x: 1,
        y: 1
    },
    draw: function() {
        console.log('draw');
    }
};

circle.draw(); // draw

/**
 *  3 members
 *    - radius
 *    - location
 *    - draw()
 * 
```
---

#### Class: circle
- properties: used to hold value 
  - radius
  - location
- method: used to define some logic
  - draw()