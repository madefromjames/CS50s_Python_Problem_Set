# Nutrition Facts
The U.S. Food & Drug Adminstration (FDA) offers downloadable/printable posters that “show nutrition information for the 20 most frequently consumed raw fruits … in the United States. Retail stores are welcome to download the posters, print, display and/or distribute them to consumers in close proximity to the relevant foods in the stores.”

In a file called nutrition.py, implement a program that prompts consumers users to input a fruit (case-insensitively) and then outputs the number of calories in one portion of that fruit, per the FDA’s poster for fruits https://cs50.harvard.edu/python/2022/psets/2/nutrition/Nutrition-Information-for-Raw-Fruits---small-PDF-Poster.pdf. Capitalization aside, assume that users will input fruits exactly as written in the poster (e.g., strawberries, not strawberry). Ignore any input that isn’t a fruit.

Hints:

Rather than use a conditional with 20 Boolean expressions, one for each fruit, better to use a dict to associate a fruit with its calories!

If k is a str and d is a dict, you can check whether k is a key in d with code like:

if k in d:
    ...
    
Take care to output the fruit’s calories, not calories from fat!

# How to Test
Run your program with python nutrition.py.
Type Apple and press Enter. Your program should output:
Calories: 130   
Type Avocado and press Enter. Your program should output:
Calories: 50
Type Sweet Cherries and press Enter. Your program should output
Calories: 100
Type Tomato and press Enter. Your program should output nothing.

Be sure to try other fruits and vary the casing of your input. Your program should behave as expected, case-insensitively.
