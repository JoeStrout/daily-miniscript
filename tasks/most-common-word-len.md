# What's the most common word length in English?

Tags: minimicro, farmtronics

Read `/sys/data/englishWords.txt`, and print the number of words of each length between 1 and 12.  What length is most common?
Bonus: draw a little bar chart representing the number of words of each length.

<details>
<summary>Hints</summary>
This is similar to [5-letter words](5-letter-words.md), but you will need a list initialized to 13 zeros.  Why 13?  So you can ignore element 0, and use the word length as the index into the list.  Alternatively, you could use a map.

As you get the length of each word, add 1 to the corresponding count in your list or map.

After you've iterated over all the words, print the count for each length.  To make a bar chart, simply print `"="` times the length, divided by some factor chosen so that the largest bar fits on the screen.

</details>

