# Audio, Video, Images

## Images

You can control the size of an image using the width and height properties in CSS, just
like you can for any other box.Specifying image sizes helps pages to load more smoothly
because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.

In the CSS, you add selectors for each of the class names, then use the CSS width and height properties to control the image dimensions.

Rather than using the `<img>` element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:

1. The float property is added
to the class that was created to
represent the size of the image.

2. New classes are created with
names such as align-left or
align-right to align the images
to the left or right of the page.
These class names are used in
addition to classes that indicate
the size of the image.

By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a blocklevel
element using the display property with a value of block. Once it has been made into a
block-level element, there are two common ways in which you can horizontally center an image:

1. On the containing element,
you can use the text-align
property with a value of center.

2. On the image itself, you can
use the use the margin property
and set the values of the left and
right margins to auto.

The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box.

The background-repeat property can have four values:

1. repeat
The background image is
repeated both horizontally and
vertically (the default way it
is shown if the backgroundrepeat
property isn't used).
2. repeat-x
The image is repeated
horizontally only (as shown in
the first example on the left).
repeat-y
The image is repeated vertically
only.
3. no-repeat
The image is only shown once.
The background-attachment
property specifies whether a
background image should stay in
one position or move as the user
scrolls up and down the page. It
can have one of two values:
4. fixed
The background image stays in
the same position on the page.
5. scroll
The background image moves
up and down as the user scrolls
up and down the page.

When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed.This property usually has a pair of values. The first represents the horizontal position and the second represents the vertical.

The background property acts like a shorthand for all of the other background properties you have just seen, and also the background-color property.
The properties must be specified in the following order, but you can miss any value if you do not want to specify it.

1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position

CSS3 is going to introduce the ability to specify a gradient for the background of a box. The gradient is created using the background-image property and, at the time of writing, different browsers required a different syntax.Since it is not supported by all browsers, it is possible to specify a background image for the box first (which would represent the gradient) and then provide the CSS alternatives for browsers that support gradients.

If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible.

## Audio, Video

HTML5 comes with elements for embedding rich media in documents video and audio which in turn come with their own APIs for controlling playback, seeking, etc. This article shows you how to do common tasks such as creating custom playback controls.

* HTML5 introduces new `<video>` and `<audio>` elements for adding video and audio to web pages, but these are only supported in the latest browsers.

* Browsers that support the HTML5 elements do not all support the same video and audio formats, so you need to supply your files in different formats to ensure that everyone can see/hear them.

* The whole player is wrapped in a `<div>` element, so it can all be styled as one unit if needed.
* The `<video>` element contains two `<source>` elements so that different formats can be loaded depending on the browser viewing the site.

* The controls HTML is probably the most interesting:

* We have four `<button>`s — play/pause, stop, rewind, and fast forward.

* Each `<button>` has a class name, a data-icon attribute for defining what icon should be shown on each button (we'll show how this works in the below section), and an aria-label attribute to provide an understandable description of each button, since we're not providing a human-readable label inside the tags. The contents of aria-label attributes are read out by screenreaders when their users focus on the elements that contain them.

* There is also a timer `<div>`, which will report the elapsed time when the video is playing. Just for fun, we are providing two reporting mechanisms — a `<span>` containing the elapsed time in minutes and seconds, and an extra `<div>` that we will use to create a horizontal indicator bar that gets longer as the time elapses. To get an idea of what the finished product will look like

### Implementing the CSS

We start off with the visibility of the custom controls set to hidden. In our JavaScript later on, we will set the controls to visible, and remove the controls attribute from the `<video>` element. This is so that, if the JavaScript doesn't load for some reason, users can still use the video with the native controls.
We give the controls an opacity of 0.5 by default, so that they are less distracting when you are trying to watch the video. Only when you are hovering/focusing over the player do the controls appear at full opacity.
We lay out the buttons inside the control bar using Flexbox (display: flex), to make things easier.

### Implementing the JavaScript

1. Create a new JavaScript file in the same directory level as your index.html file. Call it custom-player.js.

2. At the top of this file, insert the following code:
 const media = document.querySelector('video');
 const controls = document.querySelector('.controls');
 const play = document.querySelector('.play');
 const stop = document.querySelector('.stop');
 const rwd = document.querySelector('.rwd');
 const fwd = document.querySelector('.fwd');
 const timerWrapper = document.querySelector('.timer');
 const timer = document.querySelector('.timer span');
 const timerBar = document.querySelector('.timer div');

3. Next , insert the following at the bottom of your code:

media.removeAttribute('controls');
controls.style.visibility = 'visible';

These two lines remove the default browser controls from the video, and make the custom controls visible.

Playing and pausing the video

1. First of all, add the following to the bottom of your code, so that the playPauseMedia() function is invoked when the play button is clicked.

2. Now to define playPauseMedia() — add the following, again at the bottom of your code.

### Resources used in this reading

1. duckett_html.
2. <https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs>
