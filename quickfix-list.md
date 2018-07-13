# Quickfix list

## Building

Command | Keystrokes | Comments
------- | ---------- | --------
Run make (and jump to first error, if there are any) | `:make`
Run make (and stay where we are) | `:make!` | if you forgot and have moved, you can use `<c-o>`

## Navigating Quickfix list
Command | Keystrokes | Comments
------- | ---------- | --------
Move to next error in quickfix list | `:cnext`
Previous | `:cprev`
Move forward five items | `:5cnext`
Move back five items | `:5cprev`
First | `:cfirst`
Last | `:clast`
First item in next file | `:cnfile`
Last item in previous file | `:cpfile`
Nth item | `:cc N`
Open quickfix window | `:copen`
Close quickfix window | `:cclose`
