# How many 5-letter words are there? 

Tags: minimicro, farmtronics

Read the `/sys/data/englishWords.txt`, and count the number of 5-letter words therein.

<details>
<summary>Hints</summary>

You'll need to use the [file](https://miniscript.org/wiki/File) module to read all lines of the file.  The result will be a list, which you can iterate over with a [for loop](https://miniscript.org/wiki/For).  Check the length of each string using [len](https://miniscript.org/wiki/Len), and if that length is 5, add 1 to a counter.

</details>
