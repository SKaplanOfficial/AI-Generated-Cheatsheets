# AppleScript Cheatsheet

AppleScript is a scripting language developed by Apple Inc. for automating tasks on Mac OS X. Here is an overview of its unique features, code blocks, and resources.

## Unique Features

- AppleScript can interact with most applications on Mac OS X.
- It can be used to automate repetitive tasks, such as file management, data processing, and more.
- AppleScript can also be used to control other devices, such as iPhones and iPads.

## Code Blocks

### Variables

Variables are used to store data that can be used later in the script.

```applescript
set variableName to value
```

### Handlers

Handlers are code blocks that perform a specific task. They can be called by other parts of the script.

```applescript
on handlerName(parameter1, parameter2)
	-- code to be executed
end handlerName
```

### Conditionals

Conditionals allow the script to make decisions based on certain conditions.

```applescript
if condition then
	-- code to be executed if condition is true
else if otherCondition then
	-- code to be executed if otherCondition is true
else
	-- code to be executed if neither condition is true
end if
```

### Loops

Loops allow the script to repeat a set of instructions.

```applescript
repeat with i from 1 to 10
	-- code to be executed
end repeat
```

### File Manipulation

AppleScript can be used to manipulate files and folders on the file system.

```applescript
tell application "Finder"
	set theFiles to every file of desktop
end tell
```

### User Interface

AppleScript can be used to interact with the user interface of applications.

```applescript
tell application "System Events"
    tell process "Finder"
        click menu item "Empty Trash" of menu "Finder" of menu bar 1
    end tell
end tell
```

## Resources

Here are some resources for learning and using AppleScript:

- [AppleScript Language Guide](https://developer.apple.com/library/archive/documentation/AppleScript/Conceptual/AppleScriptLangGuide/introduction/ASLR_intro.html)
- [MacScripter](https://macscripter.net/)
- [AppleScript subreddit](https://www.reddit.com/r/applescript/)
-[AppleScript on Stack Overflow](https://stackoverflow.com/questions/tagged/applescript)