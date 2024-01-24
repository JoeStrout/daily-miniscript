# Word Search

Tags: minimicro

Find all 8-letter words hidden in a grid of letters

Download [this file](wordgrid.txt), which contains a 10x10 grid of letters that looks like this:

```
DVLANGUAGE
DIDUGRUUHA
MCSNMEYQAF
IOACWILUPR
NMMWONUMPE
IPPZDVEMIE
MUBWCEEVEW
ITBWONNRSA
SEZLNTMTTR
ERELIABLEE
```

Hidden in this grid are eight 8-letter words.  They may appear horizontally, vertically, or diagonally.

Sure, you could search for them yourself, but why work so hard when you can code instead?  Using the word list at /sys/data/englishWords.txt, write a program to find all the 8-letter words in this grid.

<details>
<summary>Hints</summary>

Start by reading the grid using [file.readLines](https://miniscript.org/wiki/File.readLines).  Filter that list down to just the 8-letter words, either by [import](https://miniscript.org/wiki/Import)ing "listUtil" and using `.filter`, or just by using a loop.

Write a function to return the string of letters that start at a given x,y position in the grid, and extend in a given dx,dy direction.

Then, you can loop over all grid positions — and over all directions — using nested `for` loops.  Get the string of letters at that position and orientation, and if it's longer than 8 letters, trim it to just 8.  Then just see if that string of letters (converted to lowercase) is in your word list, and if so, print it!
</details>
