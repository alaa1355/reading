Building Blocks CSS treats each HTML

Building Blocks CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors.

Containing Elements

It is common to group a number of elements together inside a

(or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The

element that contains this group of elements is then referred to as the containing element.

Normal Flow

position:static

Relative Positioning

position:relative

Absolute Positioning

position:absolute

position:fixed

# Overlapping Elements

z-index

When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page.

**Floating Elements**

The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.

**Clearing Floats**

The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:

1. Left
2. Right
3. Both
4. None

**Parents of Floated Elements: Problem**

If a containing element only contains floated elements, some browsers will treat it as if it is zero pixels tall.

As you can see in this example, the one pixel border assigned to the containing element has collapsed, so the box looks like a two pixel line.

**Parents of Floated Elements: Solution**

Traditionally, developers got around this problem by adding an extra element after the last floated box (inside the containing element). A CSS rule would be applied to this additional element setting the clear property to have a value of both. But this meant that an extra element was added to the HTML just to fix the height of the containing element.

**Creating Multi-Column Layouts with Floats**

width This sets the width of the columns.

float This positions the columns next to each other

margin This creates a gap between the columns.