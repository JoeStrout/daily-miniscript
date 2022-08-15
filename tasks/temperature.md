# Make A Temperature Unit Converter

Tags: minimicro, farmtronics, commandline

Create a program that converts between temperature units by taking a temperature, including the unit it is in (C, F, or K for Celsius, Farenheit, and Kelvin respectively), and then a target unit, and converting the orginal temperature to the target unit.

Example:
```
Temperature? 24 C
Target unit? F
24 C is 75.2 F.
```

<details>
<summary>Hints</summary>

Use ``input`` to get user input to get the temperature and units.

Use ``split`` in the process of parsing your input.

Convert to a common unit to handle conversions easier.

Conversion formulas are here: https://en.wikipedia.org/wiki/Conversion_of_scales_of_temperature#Celsius

</details>
