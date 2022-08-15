# Convert Text to Morse Code

Tags: minimicro, farmtronics, commandline

Create a program that takes a string as input and ouputs it in [https://en.wikipedia.org/wiki/Morse_code](Morse code), printing "." for each dot and "-" for each dash, with spaces between the letters.

Example:

```
Input: Hello
Output: .... . .-.. .-.. ---
```

<details>
<summary>Hints</summary>

  Use ``input`` to get the input string.

Use a map to store and fetch morse code versions of letters.

Push the code for each letter onto a list, and use ``join`` to convert that list to a string.

</details>
