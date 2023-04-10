# Emacs Cheatsheet

## Unique Features
- Extensible, customizable text editor
- Supports many programming languages and markup formats
- Includes a built-in Lisp interpreter for scripting and customization
- Can be used as a complete development environment
- Includes a wide range of built-in functionality and packages

## Buffers
```emacs
C-x b buffer_name RET
```

## Windows
```emacs
C-x 2  // Split window vertically
C-x 3  // Split window horizontally
C-x 0  // Delete current window
C-x 1  // Delete all windows except current
```

## Navigation
```emacs
C-v  // Scroll forward one screen
M-v  // Scroll backward one screen
C-l  // Center current line in window
C-a  // Move to beginning of line
C-e  // Move to end of line
```

## Editing
```emacs
C-k  // Kill (cut) text from cursor to end of line
C-y  // Yank (paste) previously killed text
C-w  // Kill region (selected text)
M-w  // Copy region (selected text)
```

## Search and Replace
```emacs
C-s  // Search forward
C-r  // Search backward
M-%  // Query replace
```

## Macros
```emacs
C-x (  // Start recording macro
C-x )  // Stop recording macro
C-x e  // Execute macro
```

## Packages
```emacs
M-x package-list-packages  // List available packages
M-x package-install package_name  // Install package
```

## Resources
- [GNU Emacs Manual](https://www.gnu.org/software/emacs/manual/)
- [EmacsWiki](https://www.emacswiki.org/)
- [Mastering Emacs](https://www.masteringemacs.org/) (blog)
- [Emacs Rocks!](http://emacsrocks.com/) (video tutorials)