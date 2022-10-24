# Convert from Decimal to Roman Numerals

Tags: minimicro, farmtronics, commandline, tryit

You have decided to start a movie company.  You quickly realize that the most difficult part will be writing the copyright year in Roman numerals in the credits.  MiniScript to the rescue!

Write a `decToRoman` function that can convert any integer from 1 to 3999 into Roman numerals using [https://en.wikipedia.org/wiki/Roman_numerals#Standard_form](standard form) (including IV for 5, IX for 9, etc.).  Check your work on the following test cases:

```
39: XXXIX
160: CLX
207: CCVII
246: CCXLVI
789: DCCLXXXIX
1009: MIX
1066: MLXVI
1776: MDCCLXXVI
2421: MMCDXXI
```

<details>
<summary>Hints</summary>

You will need a map that encodes the Roman letters for 1, 4, 5, 9, 10, 40, 59, 90, and so on up to 1000.  Then, your function will enter a loop, looking for the biggest such value that is not bigger than your number.  When you find that, add the letters to your output string, and _subtract_ that value from your number.  Repeat until the number has gone to zero.

</details>
