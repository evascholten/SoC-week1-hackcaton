# SoC-week1-hackcaton

So far, the solution will keep adding +1 to cont1 when the loop meets a new continent. 

#Initial idea

so we start looping over tiles and if it's a land tile, we keep looping as long as it has at least 1 land tile neighbour. But only checking downwards, not up I suppose, otherwise it would always have neighbours unless it's a 1x1 continent. So when a land tile has no land neighbours below or next to it, we stop adding 1 to count. We keep looping though until we find another land tile and then it starts again. However, for this second continent, we don't add 1 to count, we add it to a new word, like count2


# Next steps


If a land tile has no land neighbours below (including diagonally) and the next land tile doesn't either until the end

OR

If a land tile has zero neighbours on top

Or

Left

OR

Right

Then the loop should stop adding +1 to cont1 if it meets a new land tile. Instead, new land tiles should add +1 to cont2. Ideally, we tell the loop to create a new cont to add to when it stops adding to cont1.
