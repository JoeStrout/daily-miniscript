# Make a date calculator 

Tags: minimicro, farmtronics, commandline

Need a date?  Write a program that uses the [`dateTime` module](https://github.com/JoeStrout/minimicro-sysdisk/blob/master/sys/lib/dateTime.ms) to calculate the date for any given number of days after (or before) the current date.

![Screen shot](dateCalc.png)

<details>
<summary>Hints</summary>

Start with `import "dateTime"` (in Mini Micro, Farmtronics, or command-line MiniScript).  This provides methods to convert back and forth between two ways of representing a date/time:

1. A numeric value, the number of seconds since January 1, 2000; and
2. A string value like `"2022-08-13 14:03:39"`

The `dateTime.nowVal` and `dateTime.now` functions return the current date in each of these formats.  With the numeric format, you can simply add the number of seconds in a day, multiplied by the number of days of interest, to get the numeric representation of the target date.  Use `dateTime.str` to convert this to string format.

Finally, to print just the date and ignore the time, simply truncate the date string to the first 10 characters (using the [slice operator](https://miniscript.org/wiki/Slice)).
</details>
