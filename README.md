# jquery.stopframeanimation
The simplest yet effective jQuery stop frame animation plugin

Download
--------
* [Uncompressed](https://raw.github.com/afklondon/jquery.stopframeanimation/master/src/jquery.stopframeanimation.js)
* [Compressed](https://raw.github.com/afklondon/jquery.stopframeanimation/master/src/jquery.stopframeanimation.min.js)

Purpose
-------
Enable stop-frame-animation easily for multiple DOM elements

Usage
-----
Add either the jquery.stopframeanimation.js or jquery.stopframeanimation.min.js along with the jQuery library to your HTML document

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
<script type="text/javascript" src="jquery.stopframeanimation.min.js"></script>
```

Add all animation frames in a container element into your HTML document (it is suggested to assign "display: none;" through CSS to the frames so they are not visible until the plugin is started)

```html
<img src="frames/frame1.svg" class="animation_frame" alt="Animation frame" onerror="$(this).hide();" style="display: none;">
<img src="frames/frame2.svg" class="animation_frame" alt="Animation frame" onerror="$(this).hide();" style="display: none;">
<img src="frames/frame3.svg" class="animation_frame" alt="Animation frame" onerror="$(this).hide();" style="display: none;">
```

Then call the plugin on the container jQuery element in order to initialise and start the animation

```javascript
// attach to an element
$(".container").stopframeanimation();
```

You can set your own options when you call the plugin for first time but you can also do this later on at runtime in exactly the same way

```javascript
$(".container").stopframeanimation( {
    interval: 30 // the time each frame is shown [default: 15]
});
```

And finally that's how you unattach the script from the jQuery element

```javascript
// unattach from an element
$(".container").stopframeanimation("destroy");
```

Dependencies
-------
jQuery 1.7+ (only tested with 2.1.4)

Browser Support
-------
* IE9+
* Firefox
* Chrome
* Safari
* Opera
* iOS Safari
* Chrome Mobile
* IE Mobile
* Opera Mobile
* Opera Mini
* Blackberry Browser

Bug?
-------
Please do [submit a ticket](https://github.com/afklondon/jquery.stopframeanimation/issues/new) if you notice a bug. Thank you very much :)
