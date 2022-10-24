# Letter Value Sum

Tags: minimicro, farmtronics, commandline, tryit

Assign every lowercase letter a value, from 1 for `a` to 26 for `z`.  Write a `lettersum` function that, given a string, finds the sum of the values of the letters inthe string.

Examples:

```
lettersum("") == 0
lettersum("a") == 1
lettersum("z") == 26
lettersum("cab") == 6
lettersum("excellent") == 100
lettersum("unconstitutionally") == 264
```

**Bonus for Mini Micro and Farmtronics users**: read all the words in `/sys/data/englishWords.txt`, and print out any word (and its sum) whose letter sum is 250 or more.  You should find seven such words.

<details>
<summary>Hints</summary>

You don't need a map to get the value of each letter; you can calculate it directly from the Unicode value, using the [code](https://miniscript.org/wiki/Code) function.  Note that `"a".code` is 97.

From there, it's just a matter of using a [for loop](https://miniscript.org/wiki/For) to iterate over the letters of the given string, adding up the value for each.

</details>

This challenge was adapted from [this Reddit post](https://www.reddit.com/r/dailyprogrammer/comments/onfehl/20210719_challenge_399_easy_letter_value_sum/).
