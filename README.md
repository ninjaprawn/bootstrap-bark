#bootstrap-bark

Bootstrap Bark is a better way to send notifications to users using JQuery and Bootstrap. This is based on Bootstrap Growl.

##Features added

* Callback functions (when notification fades away)
* More coming soon.

##Dependencies

1. Latest version of jQuery. (tested on 2.1.1 and 1.11.1)
2. [Twitter Bootstrap](http://twitter.github.com/bootstrap/index.html). (current rev tested with 3.2.0)

##Usage

Include the dependencies and `jquery.bootstrap-growl.min.js` into your page and call the following:

```javascript
$.bootstrapGrowl("My message");
```

##Available Options

By default, growls use the standard 'alert' Bootstrap style, are 250px wide, right aligned, and are positioned 20px from the top right of the page.

```javascript
$.bootstrapGrowl("another message, yay!", {
  ele: 'body', // which element to append to
  type: 'info', // (null, 'info', 'danger', 'success')
  offset: {from: 'top', amount: 20}, // 'top', or 'bottom'
  align: 'right', // ('left', 'right', or 'center')
  width: 250, // (integer, or 'auto')
  delay: 4000, // Time while the message will be displayed. It's not equivalent to the *demo* timeOut!
  allow_dismiss: true, // If true then will display a cross to close the popup.
  stackup_spacing: 10, // spacing between consecutively stacked growls.
  callback: function() {} //callback function after notification fades away!
});
```
