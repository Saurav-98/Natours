1 - Reset CSS, add Linear gradient on the Header and make a clip path for header container.

2 - add logo and heading text at the center of the header container.

3 - adding animations for the entry of the Primary heading.

<!-- ***** backface-visibility: hidden; *********** -->

4 added Button and some animations
5 - advance button animations on hover using after pseudo class

<!-- ***********   animation-fill-mode: backwards;  ********* -->

6 - Adding Sass to project using Npm
7 - Implementing 7-in-1 Sass Architecture

1 - base - - \_base.scss - \_animations.scss - \_typography.scss - \_utlities.scss
2 - abstracts - - \_variables.scss - \_mixins.scss - \_functions.scss

3 - components -

4 - layout -

5 - pages - - \_home.scss

6 - themes -
7 - vendors -

A - main.scss

8 - Setting up Grid

<!-- About Section -->

- Utility classes
- background Clip
- transform multiple propertysimultaneously
- outline offset , outline
- styling hover and non hover elements

<!-- ***** -webkit-background-clip: text;
  color: transparent; ****** -->

For using a linear background as color for heading

<!--
  &:hover &__photo:not(:hover) {
    transform: scale(0.9);
  } -->

<!-- Interactive Cards Section -->

To Learn

- Rotating Cards,
- use Perspective in CSS.
- use the backface-visibility property
- Using Background blen modes
- use Box-decration-break

<!-- Tetimonials Section -->

To Learn

- Text Flow around shapes , Shape-Outside and float
- filter
- background video
- video element
- object-fit property

<!-- Booking Section -->

To Learn

- How to implement Solid color gradients
- How the General and Adjacent sibling selectors work
- ::input-placeholder pseudo-element
- Techniques to build custom radio buttons

<!-- Footer Section -->

To Learn -

Check Box Hack
Custom animation timing function - (Cubic Bezier curves)
Solid color gradients
transform-origin

<!-- CSS POP UP -->

To Learn

- target pseudo class
  create boxes with equal height using display: table cell
  Css text column
  automatic hyphenate

<!-- Making the Website Responsive using Power of SASS -->

ORDER: Base + Typography > General Layout + Grid > Page Layout > Components

Step - 1 .

Use SASS mixins to write all media queries
Use @content and @if SASS directives

----- Use em for defining Media Query
1em = 16px
600px = 37.5em
900px = 56.25em
1200px =75em
1800px = 112.5em

/------------
DEFINE MEDIA QUERY USING MIXINS

@mixin response($breakpoint) {
@if $breakpoint == phone {
@media screen and (max-width: 37.5em) {
@content;
}
}
USE MIXIN

@include response(phone) {
font-size: 37.5%;
// 1 rem = 6px
}

-----------------/

Step 2 - Make Html font size scalable using Rem and % calculation

font-size: 62.5%; 1rem = 10px ( For Normal Desktop Screen)
font-size: 56.25%; 1rem = 9px ( For Tablet Landscape Screen)
font-size: 50%; 1rem = 8px ( For Tablet Portrait Screen)
font-size: 37.5%; 1rem = 6px ( For Mobile Phone Screen)
font-size: 75%; 1rem = 12px ( For Big Desktop Screen)
