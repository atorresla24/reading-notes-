# Class 14 reading notes

## CSS Transforms

### Transforms

Transform property comes in two settings:
- Two-dimensional - use x- and y-axis (length and width)
- Three-dimensional - uses x-, y- and z-axis (length, width, and depth)

**Rotate** value allows an object to rotate from 0 - 360 degrees
**Scale** value allows an object to change its size
  - individual axis' can also be scaled
**Translate** value will move objects in any direction it is told to move in
**Skew** value distorts objects on the x- or y-axis 

By combining these elements 3-d figures can be made like a cube

Perpsective is another value that can be created to give the effect of depth

## CSS Transitions and Animations

### Transitions and Animations

For a transition to take place an element must have a change in state (:hover, :focus, :active, :target)

There are four transition related properties:
- **transition-property** - determines exactly what properties will be altered in conjunction with the other transitional properties
- **transition-duration** - determines the duration in which a transition takes place
- **transition-timing-function** - determines the speed of the transition
- **transition-delay** - a delay can also be set to put a time value in which the transition will not occur

### Animations

Allows to set multiple points of an element undergo a transition

Use *@keyframes*, will include name, breakpoints, and properties

## 8 simple CSS3 transitions that will wow your users

1. Fade in {
  .fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
}
2. Change color{
  .color:hover
{
        background:#53a7ea;
}
}
3. Grow and Shrink{
  .grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
}
4. Rotate elements{
  .rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}
} 
5. Square to circle{
  .circle:hover
{
        border-radius:50%;
}
}
6. 3D shadow{
  .threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}
}
7. Swing{
  @-webkit-keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
       transform: translateX(-5px);
    } 
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
@keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
        transform: translateX(-5px);
    }
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
}
8. Inset border{
  .border:hover
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}
}

## Things I want to know more about

* I want to be able to learn more about transitions and animations and being able to make more complex annimations to really make my page stand out



