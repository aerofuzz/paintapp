Drawing UI
=======

Created by Jonathan
------------

### Project goal

The goal of this project is drawing with mouse, change color of brush and size.


here is an exerpt of javascript
```javascript
function Paint() {
    ctx = document.getElementById('brushBox').getContext("2d");

    $('#brushBox').mousedown(function (e) {
        mousePressed = true;
        Draw(e.pageX - $(this).offset().left, e.pageY - $(this).offset().top, false);
    });

    $('#brushBox').mousemove(function (e) {
        if (mousePressed) {
            Draw(e.pageX - $(this).offset().left, e.pageY - $(this).offset().top, true);
        }
    });

    $('#brushBox').mouseup(function (e) {
        mousePressed = false;
    });

    $('#brushBox').mouseleave(function (e) {
        mousePressed = false;
    });
}
```
<<<<<<< HEAD
![WebSite](./README.PNG)
=======
[image]
>>>>>>> e0c3e5f8c2dd927602e43ee31c74280d653cb771
