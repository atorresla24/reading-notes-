# Class 08 reading-notes

## Learn CSS- Layout

### Display property

* Display property does two things: It determines if the box is applied to acts such as inline or block
* Inline elements behave like words in a sentence
* An explicit width and height can't be set on inline elements
* Block elements don't sit next to each other
* A block element will expand to the full width of the horizontal writing mode
* Display element also determines how an element's children should behave
* With the flex attribute all the children are converted to flex items and this allows for control over alignment, ordering and flow

### Flexbox and Grid

* Two main layout mechanisms:
  - flexbox is a layout mechanism for one-dimensional layout
    * by default will align element's children next to each other in the inline direction (either horizontal or vertical)
    * Useful mechanism for responsive web design
  - grid is designed to control multi-axis layouts 
    * Gives precise control over items' placement in two dimensions
    * Can turn into either row or column
* With (inline-block) gives a box that has some characteristics of a block but flow with inline

### Floats

* **Float** instructs element to "float" to the direction specified 

* For long lists, multi-column layouts can be made
* Position controls position on the page and works outside of normal flow

## Chapter 15: Layout

## Chapter 15: Layout

* Key Focuses:
  - Explore different ways to position elements using normal flow, relative positioning, absolute positioning and floats
  - Discover how various devices have different screen sizes and resolution and how it will affect design process
  - Learn difference between fixed and liquid layouts and how they are created
  - Find out how designers use grids to make pages look more professional
* Building blocks
  - Block-level elements
  - inline elements
* Types of positioning:
  - Normal flow
  - Relative positioning
  - Absolute positioning
* Box offset:
  - fixed positioning
  - floating elements
* Elements can be overlapped with z-index
* Float can place elements side-by-side
* Clear elements makes it so no element can touch the left or right hand sides of the boxes:
  - left
  - right
  - both
  - none
* Columns are achieved by using (div) for each column and using attributes such as width, float, and margin to alter it
* Design needs to be universal to accomodate different screen sizes
* Web designers try and make pages between 960-1000 pixels to accomodate screen size and resolution
### Fixed Layouts:

* Advantages:
  - pixel values are accurate at controlling size and positioning elements
  - designer has greater control over appearance
  - lengths of lines of text can be controlled
  - size of image will always remain the same

* Disadvantages:
  - Can end up with bigger gaps around edge of page
  - If screen is much higher resolution than designer's screen then page can look smaller and text can be harder to read
  - If font-size is increased then text might not allocate spaces properly
  - Design works best on devices that have a site or resolution that is similar to desktop or computer of the designer
  - Page will often take up more vertical space than a liquid layout with same content

### Liquid layouts:

* Advantages:
  - Pages expand to fill entire browser window 
  - If user has small window th page can contract to fit it
  - Design is tolerant of users setting font sizes larger 

  * Disadvantages:
    - if width of sections of the page isn't controlled then the design can look very different
    - If user has wide window then lines of text can become very long
    - If user has small window then lines can be squashed
    - If a fixed width item is in a box the image can overflow into text

* Grids allow for consistency and fluidity

## Things I want to know more about

* Being able to use float and positioning to further make my webpage appealing
* Understand the different layouts and how to utilize them to their full capabilities