## AppleScriptObjC Cheatsheet: Objective-C Interoperability

### Overview

AppleScriptObjC is a powerful framework that allows developers to write AppleScript code using Objective-C syntax. One of the key benefits of AppleScriptObjC is its ability to easily interoperate with Objective-C code. This cheatsheet focuses on the Objective-C interoperability features of AppleScriptObjC.

### Declaring Variables

#### Declaring Objective-C Variables

```objc
set myArray to current application's NSMutableArray's arrayWithObjects:"Hello", "World"
```

### Calling Objective-C Methods

#### Calling Objective-C Methods on Objects

```objc
set myArray to current application's NSMutableArray's arrayWithObjects:"Hello", "World"
set objectCount to myArray's count()
```

#### Calling Objective-C Class Methods

```objc
set myArray to current application's NSMutableArray's arrayWithObjects:"Hello", "World"
set newArray to current application's NSMutableArray's arrayWithArray:myArray
```

### Working with Objective-C Objects

#### Creating Objective-C Objects

```objc
set myArray to current application's NSMutableArray's alloc()
set myArray to myArray's initWithCapacity:10
```

#### Releasing Objective-C Objects

```objc
set myArray to current application's NSMutableArray's arrayWithObjects:"Hello", "World"
set myArray to missing value
```

### Working with Objective-C Properties

#### Getting Objective-C Property Values

```objc
set myWindow to current application's NSApplication's sharedApplication()'s mainWindow()
set windowTitle to myWindow's title()
```

#### Setting Objective-C Property Values

```objc
set myWindow to current application's NSApplication's sharedApplication()'s mainWindow()
myWindow's setTitle:"My Window Title"
```

### Working with Objective-C Constants

#### Getting Objective-C Constants

```objc
set myConstant to current application's NSApplication's NSAppKitVersionNumber
```

### Resources

- [AppleScriptObjC Programming Guide](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/ObjCScriptingGuide/Introduction/Introduction.html)
- [AppleScriptObjC Language Guide](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/ObjCScriptingGuide/ScriptingOverview/ScriptingOverview.html)
- [AppleScriptObjC Release Notes](https://developer.apple.com/library/archive/releasenotes/InterapplicationCommunication/RN-AppleScriptObjC/index.html)
- [Objective-C Programming Guide](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/ObjectiveC/Introduction/introObjectiveC.html)