# PW# DOCS

## Applying Sprites
To start, use the apply command, like this: <br>
```apply [your sprites]```<br>
If there are multiple sprites, you seperate them with `&`, like:<br>
```apply sprite1&sprite2```<br>
## Variables
The variables are stored in runtime variables.<br>
You can set, change, and delete the variables.<br>
Use it like this:<br>
```var.set:name=value```<br>
```var.change:name=value```<br>
```var.del=name```<br>
You will notice a lot of commands are seperated by a `=`, this is for simplicity.<br>
You can also call these variables. This is covered more in the ``Inputs`` section.<br>
You call them by calling a single-command input, with `!`, like ```!xof:sprite```.<br>
To call the variable, you use `$`, so it would be `!$variable`.<br>
When calling the variable during an operation, you want it to be a `$` sign,<br>
like this: ```($variable \+ 5)```.<br>
## Inputs
The inputs are designed to be simple, not fast. Big operations will take time.<br>
To start doing an operation, use parenthathes. The program doesnt use them,<br>
they are just there to tell it is an operation.<br>
Current commands are:<br>
```# \+ #```, ```# \- #```, ```# \* #```, ```# \/ #```, ```# \rand #```<br>
They should all be self-explanitory.<br>
The \ is there so the program knows how many operations there actually is.<br>
```\rand``` is used to generate a random number from the first number to the last number.<br>
```1 \rand 10``` outputs a random integer between 1 and 10.<br>
#### Single Inputs
Single inputs are inputs that takes only 1 statement in, and gives 1 statement out.<br>
To call them, use `!` instead of paranthethes.<br>
The current commands (examples of) are:<br>
```$variable```, ```id```, ```xof:spritename```, ```yof:spritename```<br>
They can all be called mid-operation, but then you dont need a `!` in front.<br>
You can use them like ```(id + $var)``` too.<br>

## Movement
To move sprites you can use the commands:
```move.X/Y=speed```, ```move.F=speed```, ```goto.X/Y=coordinate```, <br>
```turn.r/l=degrees```, ```dir.casual=direction``` <br>
To understand the syntax you need to understand the intention behind <br>
every name. The F in ```move.F=speed``` indicates it is to move forward, <br>
r/l in ```turn.r/l=degrees``` is for right or left. The casual in ```dir.casual=direction``` <br>
means it is a casual shift in direction to a certain amount of degrees. <br>
These can of course be used together with inputs, like for example: <br>
<br>
```goto.X=(pipe1 \- 90)``` <br>
> Used in my flappy bird clone <br>
The directions are using the traditional rose compass <br>
