# Lokasenna's Lua snippets

Nothing particularly impressive at the moment; just a few things I have to type out in almost every script I write.

### msg
The standard wrapper for ```reaper.ShowConsoleMsg``` that most of us use.

### dmsg
The same, but with a global flag (```dm = true```) to determine if messages will be printed or not. Useful if you want to leave your debug messages in a released script without necessarily printing them on the end-user's screen.

### reapack
A blank ReaPack header.

### head
A simple ASCII block to use for headings in comments, just for better visual separation.