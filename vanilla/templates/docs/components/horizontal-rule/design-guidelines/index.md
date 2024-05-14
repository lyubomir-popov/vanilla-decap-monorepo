---
wrapper_template: _layouts/docs.html
context:
  title: Rule | Design Guidelines
  status: braindump
---
The horizontal rule is one of the most important elements in our layouts.

* It indicates the beginning of a new group of elements. This might be a top level section of a page, or a smaller set of elements, which form a subset within a larger group.
* It “anchors” elements that are far apart, and at risk of appearing floating in space.
* Can be used to indicate thee place within the page’s hierarchy where the content belongs


## Anatomy

A horizontal rule consists of a line with an optional margin. It has a couple of variations in terms of colour and line-width.


## Variations


#### Color

We have 3 levels of prominence: 



* Highlight: Used to make a section stand out. We use a combination of increased thickness and contrast, as in these stats:

![alt_text](https://assets.ubuntu.com/v1/e6db2a9a-Screenshot%202024-05-14%20at%2012.22.56.png "image_tooltip")

* Default: This is the most used case for top level sections on a page or in an app:

![alt_text](https://assets.ubuntu.com/v1/6cb361af-Screenshot%202024-05-14%20at%2012.03.34.png "image_tooltip")


* Muted: Secondary hrs within a section use lighter contrast (aided by column indentation) to indicate the content it accompanies is nested within a more complex hierarchy. Compare the horizontal rule that start in the first column vs the ones above buttons and links/smaller text (muted):

![alt_text](https://assets.ubuntu.com/v1/b57d5d1d-Screenshot%202024-05-14%20at%2012.04.06.png "image_tooltip")

#### Line width

Horizontal lines can be either thick or thin (see examples above). 

Thick rules should always use the highlight colour. Therefore, is-highlighted and is-muted should never be applied together on the same element.

#### Spacing

##### With spacing

By default, horizontal rules have a small margin-bottom (.5rem) to ensure it doesn’t touch things like buttons or images. This should be the only situation in which we use the margin-bottom.

##### Without spacing

In most cases, when placed above text, the margin-bottom is not needed. All text elements have padding-top so additional space is not needed. We use the “p-rule” class to remove the margin in these cases.

##### What not to do

* Avoid inserting large amounts of white space between a horizontal rule and the elements it anchors. As an example of what not to do,. The horizontal rule no longer helps guide the eye from the logo to the text, everything feels floaty, and the whole layout looks padded to the point of being baby-proofed:

![alt_text](https://assets.ubuntu.com/v1/b57d5d1d-Screenshot%202024-05-14%20at%2012.04.06.png "image_tooltip")

* Use muted vs non-muted hrs consistently as described above, based on the place within the page hierarchy. 
