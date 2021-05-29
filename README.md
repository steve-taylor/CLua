# CLua

This is a slightly modified version of Lua, made for embedding in iOS and macOS apps via Swift Package Manager.

**Important:** I created this for personal use. If you want to use it, fork it and compare it to the original Lua source code to ensure it is safe to use.

## Modifications to Lua

To ensure portability across all Apple's platforms, the following functions have been removed from `loslib.c`:

* `os_execute`
* `os_exit`

Additionally, the following files have been removed as they're unnecessary for embedding Lua:

* `lua.hpp`
* `lua.c`
* `luac.c`
