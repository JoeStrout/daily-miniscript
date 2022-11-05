# Anagram Finder

Tags: minimicro, farmtronics

Ask the user to enter a word.  Print out all the words in `/sys/data/englishWords.txt` which are anagrams of the entered word — that is, which use the same letters, but possibly in a different order.

For example, if the input is "break", then the program should print *baker*, *brake*, and *break*.

<details>
<summary>Hints</summary>

You'll need to use the [file](https://miniscript.org/wiki/File) module to read all lines of the file.  The result will be a list, which you can iterate over with a [for loop](https://miniscript.org/wiki/For), checking whether each one is an anagram of the entered word.

To do that check, make a list of the letters in the entered word (using `split`).  Then iterate over the letters of the word under consideration.  If the letter is not found in your list, bail out; otherwise, remove it from the list.  After all that, if the list is empty, the word is an anagram of the entered word; otherwise it is not.

</details>
