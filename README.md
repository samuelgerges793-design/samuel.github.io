# samuel.github.io
CPAN-133-0ND Project

Project: Unit Converter

About:

The Unit Converter is a menu-driven shell script that converts values between common units of measurement. Users choose a conversion type from a simple menu, enter a value, and get the result right away in the terminal. The script runs in a loop, so users can do as many conversions as they want without restarting the program. It uses core shell scripting concepts such as variables, functions, case statements, loops, and file handling. The goal of this project is to build a practical, easy-to-use tool while showing our understanding of Bash scripting.

Features:

1. **Input Validation** – Before any conversion happens, the script checks that the user has entered a valid number. If the input contains letters, symbols, or is left blank, an error message is shown and the user is asked to try again. This stops the script from crashing or giving incorrect results. Both whole numbers and decimals, including negative values, are accepted.

2. **Conversion History** – Every conversion is saved to a history file along with the date and time it was made. Users can view their past conversions at any time from the main menu. There is also an option to clear the history and start fresh. This feature shows how shell scripts can read from and write to files.

3. **Two-Way Conversion** – Each unit pair can be converted in both directions, such as kilometers to miles and miles to kilometers. This gives users more flexibility without needing a separate tool for each direction. The reverse conversion uses the same conversion factor, dividing instead of multiplying. This approach keeps the code short while doubling the number of available conversions.

4. **Decimal Precision** – Users can choose how many decimal places they want their results to show, from 0 to 4. This keeps the output clean and easy to read instead of showing long decimal numbers. The script uses the `bc` command to handle the math and `printf` to round the final result. This is especially useful when exact values matter or when a quick estimate is enough.
