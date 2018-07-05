# Vim-fugitive notes

## Checking git status

Operation | Keystrokes | Comments
--------- | ---------- | --------
Status | `:Gstatus` |
Jump to next file (in Gstatus buffer) | `<c-n>`
Jump to previous file (in Gstatus buffer) | `<c-p>`
For file(s) under cursor (in Gstatus buffer), add to/remove from git index | '-' | multiple files can be added/removed in visual mode.  Not that `:Git add .` is faster if you have a lot of files
Open file under cursor | <CR> | 

## Staging and unstaging

Operation | Keystrokes
--------- | ----------
Stage current file | `:Gwrite`
Revert *uncommitted* changes on current file | `:Gread`

Might be worth trying to grok fugitive's notion of reading and writing.

## Committing

Operation | Keystrokes
--------- | ----------
Open commit window | `:Gcommit`

Note that you can use `<c-n>` to auto-complete.  All text in all open buffers should be available to you.

## Pulling and pushing

Operation | Keystrokes
--------- | ----------
Pull changes for current branch | `:Gpull`
Push changes for current branch | `:Gpush`

## Blame-storming

Operation | Keystrokes
--------- | ----------
Who wrote this code? | `:Gblame`

## Moving and removing files

Operation | Keystrokes
--------- | ----------
Remove current file (and buffer) | `:Gremove`
Move current file (and buffer) to `<target-path>` | `:Gmove <target-path>`

Note that `<target-path>` is relative to path of current file.

Note also that if you use an absolute path (e.g. `/target-path/`), it is relative to the root of the git repository, not the root of the file system.

