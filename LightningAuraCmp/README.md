# Lightning Aura Components Fundamentals

```javascript
var btnMessage = btnClicked.get("v.label"); // the button's label
component.set("v.message", btnMessage);     // update our message
```

Pattern in aura components: get values from child components and set values in the component itself.
