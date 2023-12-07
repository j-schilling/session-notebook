# Grid

## parent

display: grid;
gap: 20px;
grid-template-columns: 200px 200px 200px 200px
or better
grid-template-columns: repeat (4, 1fr)
grid-template-columns: 1fr 1fr 1fr;
grid-template-columns: repeat(auto-fill, 200px) <--200px is the width of an item
grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); smoother transition

fr only in available in grid -> fraction -> takes the space available.

## child

grid-column: span 2;
grid-column-start: 1;
grid-column-end: 3;
combined:
grid-column: 1 / 3;
or
grid-column: 1 / span 2;

grid-row-start: 1;
grid-row-end: 3;
grid-column-end: -1; <-- end of all columns

max-height: 300px;

object-fit: cover;

## Parent

grid-template-areas:
"web web ux da" <--define
"ds wdg wdg da"

grid-auto-columns: 1fr; <-- sets the width to be 1fr --> evens out the columns
grid-auto-rows:

# Child

grid-area: web; <--assign
