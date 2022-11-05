# Autocomplete

Tags: minimicro, farmtronics

Write a program that prompts the user to enter a (partial) word, and then prints all the words in `/sys/data/englishWords.txt` that start with that input.  For example, if the user enters "awes", the program should print *awes*, *awesome*, *awesomely*, *awesomeness*, and *awestruck*.

<details>
<summary>Hints</summary>

You'll need to use the [file](https://miniscript.org/wiki/File) module to read all lines of the file.  The result will be a list, which you can iterate over with a [for loop](https://miniscript.org/wiki/For) and see if it starts with the user's input.

The easiest way to check that would be to first `import "stringUtil"`, so then you can use the `.contains` method.  Alternatively, you could just check whether (1) the word under consideration is at least as long as the input word, and (2) a substring of the word, up to the length of the input word, equals the input word.

</details>
