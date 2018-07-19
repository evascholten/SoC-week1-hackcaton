# Initial idea for SoC-week1-hackcaton

Start looping over tiles and if it's a land tile, keep looping and adding +1 to cont1 as long as the land has at least 1 land tile neighbour. But only checking downwards, not up I suppose, otherwise it would always have neighbours unless it's a 1x1 continent. So when a land tile has no land neighbours below or next to it, stop adding +1 to cont1. Keep looping though until you find another land tile and then it should start again with checking for neighbours. However, for this second continent, don't add +1 to cont1, +1 should be added to cont2.

# Problem

So far, the solution will keep adding +1 to cont1 when the loop meets a new continent.

# Next steps

If a land tile has no land neighbours below (including diagonally) and the next land tile doesn't either until the end

OR

If a land tile has zero neighbours on top

Or

Left

OR

Right

Then the loop should stop adding +1 to cont1 if it meets a new land tile. Instead, new land tiles should add +1 to cont2. Ideally, we tell the loop to create a new cont to add to when it stops adding to cont1.
