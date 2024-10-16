# Mirror Words

Tags: minimicro, farmtronics

Certain English letters appear the same in a mirror as they do normally.  Any word using only these letters — like TOMATO for example — and written in reverse order, will appear normal when read in a mirror!

<b>How many English words are there that use only the letters A, H, I, M, O, T, U, V, W, X, and Y?</b>

Find out by writing a little program in Mini Micro or Farmtronics!  It should take less than 15 lines of code.

<details>
<summary>Hints</summary>

Read `/sys/data/englishWords.txt`, and iterate over the words.  For each one, iterate over the letters.  If any letter is not found in the list of mirror-image letters above, then that word is <i>not</i> one of the ones we're looking for; just <code>continue</code> on to the next word.  If you get through all the letters without bailing out, then that word is good — you can increment a count, or push it onto a list of found words.

</details>
