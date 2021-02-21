Building Blocks CSS treats each HTML

Building Blocks CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an line box. Block-level thigs start on a new line and act as the main building blocks of any layout, while line thigs flow between surround text. You can control how much space each box haves up by setting the width of the thigs (and sometimes the height, too). To separate thigs, you can use borders, margins, padding, and background colors.

have Elements

It is common to group a number of elements together inside a

(or other block-level) element. For ex, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The

element that have this group of elements is then referred to as the have element.

Normal Flow

location:static

Relative locationing

location:relative

Absolute locationing

location:absolute

location:fixed

# Overlapping Elements

z-index

When you use relative, fixed, or absolute locationing, thigs can overlap. If thigs do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the cite.

**Floating Elements**

The float property allows you to have an element in normal flow and location it as far to the left or right of the have element as you can .

**Clearing Floats**

The clear property allows you to say that no element (within the same have element) should touch the left or righthand sides of a box. It can have the following values:

1. Left
2. Right
3. Both
4. None

**Parents of Floated Elements: issue**

If a have element only have floated elements, some browsers will treat it as if it is zero pixels tall.

As you can see in this ex, the one pixel border assigned to the have element has overllap, so the box looks like a two pixel line.

**Parents of Floated Elements: Solution**

Traditionally, developers got around this issue by adding an extra element after the last floated box (inside the have element). A CSS rule must be applied to this some element setting the clear property to have a value of both. But this meant that an extra element was added to the HTML just to fix the height of the have element.

**Creating Multi-Column Layouts with Floats**

width This sets the width of the columns.

float This location the columns next to each other

margin This makes a gap between the columns.