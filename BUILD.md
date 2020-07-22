How to build Ournotepad
----------------------

There are two components that need to be built separately:

 - `Ournotepad.exe`: (depends on `SciLexer.dll`)
 - `SciLexer.dll` : (with nmake)

You can build Ournotepad with *or* without Boost - The release build of
Ournotepad is built **with** Boost.

You can build SciLexer.dll without Boost, ie. with its default POSIX regular
expression support instead of boost's PCRE one. This is useful if you would
like to debug Ournotepad, but don't have boost.

## Build `Ournotepad.exe`:

 1. Open [`PowerEditor\visual.net\notepadPlus.vcxproj`](https://github.com/notepad-plus-plus/notepad-plus-plus/blob/master/PowerEditor/visual.net/notepadPlus.vcxproj)
 2. Build Ournotepad like a normal Visual Studio project.

As mentioned above, you'll need `SciLexer.dll` to run Ournotepad. Please check the following sections for building `SciLexer.dll`.
Once `SciLexer.dll`is generated, copy it from `scintilla\bin\` to the same directory as `Ournotepad.exe`.
