# Lesson 4: Wile Loops

# Coding Tools

## While Loops

Similar to for loops, while loops iterate over a block of code until a condition is met. Unlike for loops, there is only one part (condition) instead of three. The syntax for a while loop is shown below:

```
while (condition)
{
	// code block to be executed
}
```

The condition in the while loop is a boolean condition just like the second part of a for loop. If the condition evaluates to true, the while loop runs another iteration. If the condition evaluates to false, the while loop stops running.

**examples**

```
while (true)
{
	// code block to be executed
}

// This while loop will run forever
```

```
while (false)
{
	// code block to be executed
}

// This while loop will never run
```

```
int my_number = 0;
int i = 0;

while (i < 10)
{
	my_number++;
}

// This while loop will run forever
```

```
int my_number = 0;
int i = 0;

while (i < 10)
{
	my_number++;
	i++;
}

// This while loop will run 10 times.
// my_number will be 10 once it is complete
```

```
int state = 1;

while (state == 1)
{
	state = digitalRead(6);
	delay(10);
}

// This while loop will run until the button connected to pin 6 is pressed
```

# Requirements

For this lesson, use the same electrical components as in lessons 1 and 3 with the same wiring minus the button (you can leave the button there if you want, but we will not be using it)

This lesson will be exactly the same as lesson 3, but using while loops instead of for loops.

There will be two while loops. One increments from 0 to 255, increasing the duty cycle so that the LED keeps getting brighter. Place a 10 millisecond delay in the while loop. The second decrements from 255 to 0, decreasing the duty cycle so that the LED keeps getting dimmer. Place a 10 millisecond delay in the while loop. The end result should be that the LED keeps getting brighter and dimmer over and over again. A template to help you get started is below.

```
void setup()
{
  // configure pin 5

}

void loop()
{
  // Create a while loop that goes from 0 to 255. It should make the LED get gradually brighter

  // Create another while loop that goes from 255 to 0. It should make the LED get gradually dimmer.
}
```
