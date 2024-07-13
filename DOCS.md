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
