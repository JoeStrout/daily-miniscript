# Broken Spacebar 

Tags: minimicro, farmtronics, commandline, tryit

You have a friend whose spacebar on their keyboard has stopped working!  And they desperately need to take some notes about the behavior of the local animals.  Fortunately, everything they might need to type is composed of these words:

	words = ["the", "a", "an",
	"fox", "foxes", "dog", "dogs", "ape", "apes",
	"ran", "walked", "jumped", "sped", "passed", "rant",
	"over", "under", "through", "past", "about",
	"new", "quick", "brown", "lazy", "sleepy", "overt",
	]

Write a program that inputs a sentence composed of these words, with no punctuation or spaces.  It should figure out what the words are, and print the corrected sentence with spaces inserted between the words.  (If there is more than one valid interpretation, any one will do.)

Here are some test cases your code should handle:

>INPUT:  thequickbrownfoxjumpedoverthelazydog
>OUTPUT: the quick brown fox jumped over the lazy dog
>
>INPUT:  anewaperanpastthesleepyfox
>OUTPUT: a new ape ran past the sleepy fox
>
>INPUT:  thedogsrantaboutthelazyfoxes
>OUTPUT: the dogs rant about the lazy foxes
>
>INPUT:  foxesranpastanape
>OUTPUT: foxes ran past an ape


<details>
<summary>Hints</summary>

The easiest way to tackle this is with recursion.  Instead of thinking about making a function that can find all the words, make a function that can find just _one_ word that fits at the start of the input, and then calls itself on the rest of the string to find the remaining words.

But note that sometimes, the rest of the string won't start with a valid word.  In that case, you should throw out the first word you found as if it doesn't match at all, and keep trying other words.

In pseudocode, a sketch of your central _splitWords_ function would be:

1. If the given string is empty, return []
2. for each possible word in our word list:
   1. if s doesn't start with this word, then continue
   2. recursively call _splitWords_ on the rest of the string AFTER this word
   3. if that returned null, continue
   4. otherwise, insert this word at the front of the list, and return it
3. if we go through all words and haven't returned already, return null

Once you have this function working, it's just a matter of calling `.join` on the result to insert the spaces.  (Alternatively, you could skip the list and just use string concatenation to build the properly spaced result as you go.)

</details>
