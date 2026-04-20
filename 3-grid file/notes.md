Use Grid for structure
Use Flexbox inside Grid items

Page layout → Grid  
Navbar items → Flexbox  
_______________________________________________________________________
Flexbox (Flexible Box Layout) is a 1D layout system.
 It arranges items in:row (horizontal) OR column (vertical)
📦 Items in a line
Use Flexbox when:You want to align items in one direction

CSS Grid is a 2D layout system.
It arranges items in:rows AND columns
📊 Like a table layout
_______________________________________________________________________
✅ Use Flexbox:
Navbar
Align items center
Buttons in a row
Small UI components
✅ Use Grid:
Full page layout (like your example)
Dashboard layout
Complex positioning
_______________________________________________________________________
grid-template-columns → defines structure (widths)
defines how many columns your grid has and their widths.
grid-template-columns = how you divide space


1. Fixed + flexible
        grid-template-columns: 200px 1fr 1fr 1fr 150px;
                    FIXED FLEXIBLE COLUMNS FIXED COLUMNS(TOT=5 columns)
fr = fraction of remaining space   1fr = flexible division

2. Responsive (auto-fit + minmax)
        grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
repeat =Repeat columns automatically
auto-fit = Fit as many columns as possible in available width
minmax(150px, 1fr) =Each column:Minimum = 150px ,Maximum = 1 fraction (flexible)

3. Equal columns
        grid-template-columns: repeat(4, 1fr);
repeat=repeat column
4= 4 columns
1fr= each column takes equal space(column become | 1fr | 1fr | 1fr | 1fr |)

4. Pure fixed columns
        grid-template-columns: 100px 200px 300px;
 No flexibility, fixed layout

5. auto keyword
        grid-template-columns: auto auto auto;
 Size depends on content

grid-template-areas → defines placement (layout)
This defines how elements are placed visually
rules on grid-template-areas
1.Same name = one continuous rectangle only,Area must be continuous (no breaking){
    "nav main nav" ❌ 
    "nav nav nav" ✅ or nav nav main , shld be
}
2.Columns must match :Number of items in each row = number of columns
3.Same number of columns in every row
4.Names must match grid-area
5.Use . for empty space{
    "header header header"
    "nav main ."  #here
    "footer footer footer"
}

                “Equal columns + rectangular areas + matching names”
_______________________________________________________________________
gap: 10px;
Adds spacing between grid items

padding: 20px;
Padding = space INSIDE an element, creates space:between content and border

Feature	        Padding	        Gap
Space location	Inside element	Between elements
Affects	        One element	    Multiple elements
Used in	        Any element	    Grid / Flexbox only
Purpose	        Content spacing	Layout spacing

👉 Padding = inside space
👉 Gap = outside space (between boxes)
_______________________________________________________________________
 gird_template_area - creates names (labels) in the grid
It does NOT automatically assign elements to those positions.
to asign we want grid-area
grid-template-areas → defines map
grid-area → tells each element where to go on that map
_______________________________________________________________________
.layout > * → use for common styling 
if i want to assign all the styling to all tags we use this one

.layout > div → common rules for all boxes 📦

div = only div
 * = everything
_______________________________________________________________________
1. .layout > div  (used in grid1.css)
                .layout > div {
                    background: lightblue;
                }
Select only <div> elements inside .layout

📌 Works for:
<div class="layout">
    <div>1</div>   ✅ selected
    <div>2</div>   ✅ selected
</div>
❌ Not applied to:
<header>Header</header> ❌
<nav>Nav</nav> ❌

 2. .layout > * (used in grid.css)
                .layout > * {
                    background: lightblue;
                }
 Select ALL direct children inside .layout (any tag)

📌 Works for:
<div class="layout">
    <header>Header</header> ✅
    <nav>Nav</nav>          ✅
    <div>Box</div>          ✅
</div>
_______________________________________________________________________
in automatic_grid file :
 i didnt unders grid template-areas and gird-area, 
 it will automatically assign the grids
_______________________________________________________________________
and as sir gave on assignemt , like if we minimiz the window we hvae to see the boxes places automatically 
for that automatic assigingof the grid , we dont use grid-template-area and grid-areas
_______________________________________________________________________
grid-column and grid-row
 Used when you don’t use grid-template-areas

✅ Example:
.item1 {
  grid-column: 1 / 3;  /* spans 2 columns */
}
.item2 {
  grid-row: 1 / 3;     /* spans 2 rows */
}
Start at line 1, end at line 3

fro precise gird , we dont use grid-template-areas, we just use grid-template-columns and rows and then
assign each box individually 
_______________________________________________________________________

2. span keyword
.item {
  grid-column: span 2;
}
Takes 2 columns space

3. justify-items & align-items (inside cells)
.grid {
  justify-items: center;
  align-items: center;
}
Controls content inside each box

4. justify-content & align-content (whole grid)
.grid {
  justify-content: center;
  align-content: center;
}
Moves entire grid