# CSS Transforms, Transitions, and Animations

![transform](https://miro.medium.com/max/1800/1*_6MfwckxNfQTca9SiG8MdQ.png)

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

* Transform Syntax

`div {`
  `-webkit-transform: scale(1.5);`
     `-moz-transform: scale(1.5);`
       `-o-transform: scale(1.5);`
         `transform: scale(1.5);`
`}`

## 2D Transforms

Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.

1. 2D Rotate
The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.
`.box-1 {transform: rotate(20deg);}`

2. 2D Scale
Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.
`.box-1 {transform: scale(.75);}`

3. 2D Translate
The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.
`.box-1 {transform: translateX(-10px);}`

4. 2D Skew
The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values.
`.box-1 {transform: skewX(5deg);}`

### 3D Transforms

Using three-dimensional transforms we can change elements on the z axis, giving us control of depth as well as length and width.

1. 3D Rotate.
2. 3D Scale.
3. 3D Translate.
4. 3D Skew.

## Transitions & Animations

### Transitions

![transitions](https://coursework.vschool.io/content/images/2016/08/hover-no-transition.gif)
for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

* Transitional Property
The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

* Transition Duration
The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.

* Transition Timing
The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out.

* Transition Delay
On top of declaring the transition property, duration, and timing function, you can also set a delay with the transition-delay property. The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. As with all other transition properties, to delay numerous transitions, each delay can be declared as comma separated values.

### Animations

![animation](https://i.pinimg.com/originals/34/9f/b6/349fb611022ec7f6176d26321fce0011.gif)
Animations Keyframes
To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

## 8 SIMPLE CSS3 TRANSITIONS

1. Fade in
2. Change color
3. Grow & Shrink
4. Rotate elements
5. Square to circle
6. 3D shadow
7. Swing
8. Inset border

### Resources used in this reading

1. <http://learn.shayhowe.com/advanced-html-css/css-transforms>
2. <http://learn.shayhowe.com/advanced-html-css/transitions-animations/>
3. <http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users>