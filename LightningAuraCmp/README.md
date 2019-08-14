# Lightning Aura Components Fundamentals

```javascript
var btnMessage = btnClicked.get("v.label"); // the button's label
component.set("v.message", btnMessage);     // update our message
```

Pattern in aura components: get values from child components and set values in the component itself.

```javascript
    handleClick2: function(component, event, helper) {
        var newMessage = event.getSource().get("v.label");
        console.log("handleClick2: Message: " + newMessage);
        component.set("v.message", newMessage);
    },
    handleClick3: function(component, event, helper) {
        component.set("v.message", event.getSource().get("v.label"));
        console.log("handleClick3: Message: " + newMessage);
    }
```
