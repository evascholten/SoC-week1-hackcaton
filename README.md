# SoC-week1-hackcaton

So far, the solution will keep adding +1 to cont1 when the loop meets a new continent. 

================
WHAT'S NEEDED
================

If a land tile has no land neighbours below (including diagonally) and the next land tile doesn't either until the end

OR

If a land tile has zero neighbours on top

Or

Left

OR

Right

Then the loop should stop adding +1 to cont1 if it meets a new land tile. Instead, new land tiles should add +1 to cont2. Ideally, we tell the loop to create a new cont to add to when it stops adding to cont1.
