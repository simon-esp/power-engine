# PW# DOCS

## Applying Sprites
To start, use the apply command, like this:
```apply [your sprites]```
If there are multiple sprites, you seperate them with `&`, like:
```apply sprite1&sprite2```
## Variables
The variables are stored in runtime variables.
You can set, change, and delete the variables.
Use it like this:
```var.set:name=value```
```var.change:name=value```
```var.del=name```
You will notice a lot of commands are seperated by a `=`, this is for simplicity.
You can also call these variables. This is covered more in the ``Inputs`` section.
You call them by calling a single-command input, with `!`, like ```!xof:sprite```.
To call the variable, you use `$`, so it would be `!$variable`.
When calling the variable during an operation, you want it to be a `$` sign,
like this: ```($variable \+ 5)```.
## Inputs
The inputs are designed to be simple, not fast. Big operations will take time.
To start doing an operation, use parenthathes. The program doesnt use them,
they are just there to tell it is an operation.
Current commands are:
```# \+ #```, ```# \- #```, ```# \* #```, ```# \/ #```, ```# \rand #```
They should all be self-explanitory.
The \ is there so the program knows how many operations there actually is.
```\rand``` is used to generate a random number from the first number to the last number.
```1 \rand 10``` outputs a random integer between 1 and 10.
### Single Inputs
Single inputs are inputs that takes only 1 statement in, and gives 1 statement out.
To call them, use `!` instead of paranthethes.
The current commands (examples of) are:
```$variable```, ```id```, ```xof:spritename```, ```yof:spritename```
They can all be called mid-operation, but then you dont need a `!` in front.
You can use them like ```(id + $var)``` too.
