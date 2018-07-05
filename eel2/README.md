# EEL2 Language Support

This folder provides an EEL2 language definition for Visual Studio Code. Language definitions are required to associate code snippets with a particular language/file format, and to provide appropriate syntax highlighting.

## Installation
Clone/download this folder's contents to the following path:
- Windows _%USERPROFILE%\.vscode\extensions_
- MacOS _~/.vscode/extensions_
- Linux _~/.vscode/extensions_

Code should now automatically detect _.eel_ and _.jsfx_ files as EEL2 (for standard installations, languages are displayed in the bottom-right corner on the status bar).

One more step is required to allow detection of JSFX files with no file extension. Because Code's pattern matcher is (currently) unable to match a negative, the simplest solution is to match everything in Reaper's Effects folder. Add the following to your User Settings:
```json
"files.associations": {
    "**/REAPER/Effects/**": "eel2"
}
```
Code should now detect **all** files in the folder as EEL2.