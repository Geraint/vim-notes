# Vim-fugitive notes

Operation | Keystrokes
--------- | ----------
Status | `:Gstatus`
Stage current file | `:Gwrite`
Revert *uncommitted* changes on current file | `:Gread`

Might be worth trying to grok fugitive's notion of reading and writing.

Operation | Keystrokes
--------- | ----------
Remove current file (and buffer) | `:Gremove`
Move current file (and buffer) to `<target-path>` | `:Gmove <target-path>`

Note that `<target-path>` is relative to path of current file.

Note also that if you use an absolute path (e.g. `/target-path/`), it is relative to the root of the git repository, not the root of the file system.

Operation | Keystrokes
--------- | ----------
Open commit window | `:Gcommit`

Note that you can use `<c-n>` to auto-complete.  All text in all open buffers should be available to you.

Operation | Keystrokes
--------- | ----------
Who wrote this code? | `:Gblame`
