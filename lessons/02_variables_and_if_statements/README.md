# Lesson 2: Variables and If Statements

# Coding Tools

## Variables

Variables are used to hold values. Values can be assigned to them and then read back at a later time. However, it is not possible to assign anything to a variable because variables are declared as being a certain type when they are initialized. There are many types, but for now, focus on the basic four listed below.

- int
- float
- bool
- char

## int

The int type (short for integer) is used to store whole numbers.

**example**
```
Create a variable of int type called my_number and assign 1 to it:

int my_number = 1;

my_number can be assigned new values after it is initialized also (if it is already initialized, don't place int in front of it again):

my_number = 10;

my_number = -1;
```

## float

The float type (short for floating point number) is used to store rational numbers (with a decimal point).

**example**
```
Create a variable of float type called my_number and assign 1.23 to it:

float my_number = 1.23;

like in the int example, float can take new values after initialized:

my_number = -1.23;

my_number = 1000.99;
```

## bool

The bool type (short for boolean) is used to store binary values (true or false).

**example**
```
Create a variable of bool type called time_to_program and assign true to it:

bool time_to_program = true;

time_to_program can be assigned false also:

time_to_program = false;
```

## char

The char type (short for character) is used to store a single character (a, b, c, 1, 2, 3 etc.)

**example**
```
Create a variable of char type called my_character and assign 't' to it (characters must always be surrounded by single quotation marks):

char my_character = 't';

my_character can be assigned other values afterwards:

my_character = 'a';

my_character = '1';
```

In all the above examples, the variables could be assigned new values after beining initialized. If const (short for constant) is used before the variable initialization, it can not be modified later.

**example**
```
Create an int variable called my_number, assign it 1, and make it so that the number cannot be changed:

const int my_number = 1;

my_number = 2; // <- this will not work

NOTE: const can be used on all variables, not just int.
```

## Boolean Operations

## If Statements

If statements are used to evaluate a condition. If the condition is true, then the code inside the if statement will run. If the condition is false, then the code inside the if statement will not run.

If statements have the following syntax. Syntax is the rules in a programming language on how code must be structured to be properly understood.

```
if (condition)
{
	// code to run when condition is true
}
```

First, it is important to understand what sort of conditions could be evaluated by an if statement.

## Comparision

Operators for comparision include:

- <
- \>
- =<
- \>=
- ==

## < (less than)

- If the number to the left of the < operator is less than the number to the right, the condition will be evaluated to true.
- If the number to the left of the < operator is greater than the number to the right, the condition will be evaluated to false.
- If the numbers are equal, the condition will be evaluated to false.

**examples**
```
int my_number = 5;

if (my_number < 4)
{
	my_number = 0;
}

// my_number will equal 5 after this code runs
```

```
int my_number = 5;

if (my_number < 5)
{
	my_number = 0;
}

// my_number will equal 5 after this code runs
```

```
int my_number = 5;

if (my_number < 6)
{
	my_number = 0;
}

// my_number will equal 0 after this code runs
```

## > (greater than)

- If the number to the left of the > operator is greater than the number to the right, the condition will be evaluated to true.
- If the number to the left of the > operator is less than the number to the right, the condition will be evaluated to false.
- If the numbers are equal, the condition will be evaluated to false.

**examples**
```
int my_number = 5;

if (my_number > 6)
{
	my_number = 0;
}

// my_number will equal 5 after this code runs
```

```
int my_number = 5;

if (my_number > 5)
{
	my_number = 0;
}

// my_number will equal 5 after this code runs
```

```
int my_number = 5;

if (my_number > 4)
{
	my_number = 0;
}

// my_number will equal 0 after this code runs
```

## <= (less than or equal)

- If the number to the left of the <= operator is less than the number to the right, the condition will be evaluated to true.
- If the number to the left of the <= operator is greater than the number to the right, the condition will be evaluated to false.
- If the numbers are equal, the condition will be evaluated to true.

**examples**
```
int my_number = 5;

if (my_number <= 4)
{
	my_number = 0;
}

// my_number will equal 5 after this code runs
```

```
int my_number = 5;

if (my_number <= 5)
{
	my_number = 0;
}

// my_number will equal 0 after this code runs
```

```
int my_number = 5;

if (my_number <= 6)
{
	my_number = 0;
}

// my_number will equal 0 after this code runs
```

## >= (greater than or equal)

- If the number to the left of the >= operator is greater than the number to the right, the condition will be evaluated to true.
- If the number to the left of the >= operator is less than the number to the right, the condition will be evaluated to false.
- If the numbers are equal, the condition will be evaluated to true.

**examples**
```
int my_number = 5;

if (my_number >= 6)
{
	my_number = 0;
}

// my_number will equal 5 after this code runs
```

```
int my_number = 5;

if (my_number >= 5)
{
	my_number = 0;
}

// my_number will equal 0 after this code runs
```

```
int my_number = 5;

if (my_number >= 4)
{
	my_number = 0;
}

// my_number will equal 0 after this code runs
```

## == (equal)

- If the value on the right side of == equals the value on the left, the condition will be evaluated to true.
- If the values are not equal, the condition will be evaluated to false.

**examples**
```
int my_number = 5;

if (my_number == 5)
{
	my_number = 0;
}

// my_number will equal 0 after this code runs
```

```
int my_number = 5;

if (my_number == 10)
{
	my_number = 0;
}

// my_number will equal 5 after this code runs
```

## Logical

Logical operators include:

- &&
- ||
- !

## && (AND)

- The conditions on both side of && must be true for the enire condition to be true

**examples**
```
int my_number = 5;

if (true && true)
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

```
int my_number = 5;

if (true && false)
{
	my_number = 0;
}

// my_number will be 5 after this code runs
```

```
int my_number = 5;

if (false && true)
{
	my_number = 0;
}

// my_number will be 5 after this code runs
```

```
int my_number = 5;

if (false && false)
{
	my_number = 0;
}

// my_number will be 5 after this code runs
```

```
int my_number = 5;
int my_other_number = 10

if ((my_number < 8) && (my_other_number > my_number))
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

## || (OR)

- Only the conditions on one side of || must be true for the enire condition to be true. Both sides can also be true for the entire condition to be true.

**examples**
```
int my_number = 5;

if (true || true)
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

```
int my_number = 5;

if (true || false)
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

```
int my_number = 5;

if (false || true)
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

```
int my_number = 5;

if (false || false)
{
	my_number = 0;
}

// my_number will be 5 after this code runs
```

```
int my_number = 5;
int my_other_number = 10

if ((my_number > 8) || (my_other_number > my_number))
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

## ! (NOT)

- The ! operator reverses the condition. If the condition was true, it will be false. If the condition was false, it will be true.

```
int my_number = 5;

if (!false)
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

```
int my_number = 5;

if (!true)
{
	my_number = 0;
}

// my_number will be 5 after this code runs
```

```
int my_number = 5;

if (!(my_number > 10))
{
	my_number = 0;
}

// my_number will be 0 after this code runs
```

## More on If Statements

If statements can also have "else if" and "else" statements added to them. Else if statements are evaluated if the original if statements was false. If the if statement was evaluated to false and all else if statements (if there were any) were also evaluated to false, the code inside the else statement will be run. Once one of the statements evaluates to true, none of the else if statements or else statement below will be checked.

**example**\
Say you want someone to pick a color, and the way the user picks a color is by choosing a number. You let the user know the following information:

```
Press 0 to choose red.
Press 1 to choose yellow.
Press 2 to choose blue.
```

If the user presses 0, you could have the if statement select red as the color. There would be no reason to check if the user chose yellow or blue also because you already know the user chose red. You would not want to do this because it would be inefficient:

```
bool red = false;
bool yellow = false;
bool blue = false;

if (variable_containing_user_input == 0)
{
	red = true;
}

if (variable_containing_user_input == 1)
{
	yellow = true;
}

if (variable_containing_user_input == 2)
{
	blue = true;
}
```

This would be a better method:

```
bool red = false;
bool yellow = false;
bool blue = false;

if (variable_containing_user_input == 0)
{
	red = true;
}
else if (variable_containing_user_input == 1)
{
	yellow = true;
}
else if (variable_containing_user_input == 2)
{
	blue = true;
}
```

Say you also want to track if the user presses something other than 0, 1, or 2 to report that there was invalid input. An else statement would accompilsh this well.

```
bool red = false;
bool yellow = false;
bool blue = false;
bool invalid_input = false;

if (variable_containing_user_input == 0)
{
	red = true;
}
else if (variable_containing_user_input == 1)
{
	yellow = true;
}
else if (variable_containing_user_input == 2)
{
	blue = true;
}
else
{
	invalid_input = true;
}
```

NOTE: An else statement does not need an else if statement to come before it. There could just be an if statement and then and else statement after it.

# Requirements

For this lesson, use the same electrical components as in lesson 1 with the same wiring. The logic will be different this time:

Only when the button is released, the LED will change its state. If the LED was on, it will change to off and remain off after the button is released. If the LED was off, it will change to on and remain on after the button is released.

Below is a template to help you get started:
```
// variables should be declared at the top of the file.
int button_state = 1;
int previous_button_state = 1;
bool led_on = false;

void setup() {
  // Configure pins 5 and 6 with the pinMode function

}

void loop() {
  // Use digitalRead and digitalWrite
  // Use an if statement or two
  // You will need to use both button_state and previous_button_state variables
  // Use the led_on variable to track if the led is on or off. Then, switch it to off if it was on and vice versa.

  delay(1);
}
```

## Tips:
- Sleep time is only 1 millisecond instead of 100 in the delay function because we want to make it more likely that we catch the button state transition when it changes from being pressed to released
- HIGH returned from digitalRead is the same as an integer equal to 1. LOW returned from digitalRead is the same as an integer equal to 0.
