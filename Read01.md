# Read 1 Notes

## Floats

Link: https://css-tricks.com/all-about-floats/

Float is a CSS positioning property.

Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.

can affect the element that contains them (their “parent” element). If this parent element contained nothing but floated elements, the height of it would literally collapse to nothing. 

* Pushdown is a symptom of an element inside a floated item being wider than the float itself (typically an image). 

* Double Margin Bug – Another thing to remember when dealing with IE 6 is that if you apply a margin in the same direction as the float, it will double the margin. Quick fix: set display: inline on the float, and don’t worry it will remain a block-level element.

* The 3px Jog is when text that is up next to a floated element is mysteriously kicked away by 3px like a weird forcefield around the float. Quick fix: set a width or height on the affected text.

* In IE 7, the Bottom Margin Bug is when if a floated parent has floated children inside it, bottom margin on those children is ignored by the parent. Quick fix: using bottom padding on the parent instead.

If you need text wrapping around images, there really aren’t any alternatives for float. see https://blog.ideashower.com/post/15139639050/css-text-wrapper

# Responsive Web Design

Link: https://learn.shayhowe.com/advanced-html-css/responsive-web-design/

Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

Responsive and adaptive web design are closely related, and often transposed as one in the same. Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change. With responsive design websites continually and fluidly change based on different factors, such as viewport width, while adaptive websites are built to a group of preset factors.

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media. 

target ÷ context = result


# Floats
All about floats (https://css-tricks.com/all-about-floats/)

Floats (escalator)
https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/

# Grids
Grids (https://css-tricks.com/dont-overthink-it-grids/)


### [home](https://misalz.github.io/reading_notes2/)