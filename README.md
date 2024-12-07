# Python---Format---Strings

String Format

As we learned in the Python Variables chapter, we cannot combine strings and numbers like this:

Example

age = 36
txt = "My name is John, I am " + age
print(txt)

But we can combine strings and numbers by using f-strings or the format() method!

F-Strings

F-String was introduced in Python 3.6, and is now the preferred way of formatting strings.

To specify a string as an f-string, simply put an f in front of the string literal, and add curly brackets {} as placeholders for variables and other operations.

Example

Create an f-string:

age = 36
txt = f"My name is John, I am {age}"
print(txt)

"Placeholders and Modifiers"

A placeholder can contain variables, operations, functions, and modifiers to format the value.

Example

Add a placeholder for the price variable:

price = 59
txt = f"The price is {price} dollars"
print(txt)

A placeholder can include a modifier to format the value.

A modifier is included by adding a colon : followed by a legal formatting type, like .2f which means fixed point number with 2 decimals:

Example

Display the price with 2 decimals:

price = 59
txt = f"The price is {price:.2f} dollars"
print(txt)

A placeholder can contain Python code, like math operations:

Example

Perform a math operation in the placeholder, and return the result:

txt = f"The price is {20 * 59} dollars"
print(txt)

Exercise

If x = 9, what is a correct syntax to print 'The price is 9.00 dollars'?


print(f'The price is {x:.2f} dollars')

print(f'The price is {x:2} dollars')

print(f'The price is {x:format(2)} dollars')
