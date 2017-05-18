# Greyscale Antialiasing extension for VSCode (Mac OSX Only)

This extension is a dirty hack to permit the usage of fonts on OSX (such as ProFont) that
benefits from being displayed with greyscale antialiasing, patching the application's
main CSS file.

Althought this could be done manually, at every VSCode update the changes are lost: this
extension ensure those changes are re-applied automatically in such cases.

See: [https://github.com/Microsoft/vscode/issues/2577](https://github.com/Microsoft/vscode/issues/2577)

## Features

Here how ProFont looks with antialiasing (default behavior of VSCode):

![Before the patch](images/screenshot-default.png)

And Here after the patch is applied.

![After the patch](images/screenshot-patched.png)

## Installation

Downlod the latest extension's vsix package [here](https://github.com/legoadk/slightly-less-roughify/releases/download/v0.0.3/slightly-less-roughify-0.0.3.vsix).

From the terminal, you can install using the following command:

```
$ code --install-extension slightly-less-roughify-0.0.3.vsix
```

## Requirements

Due the nature of the CSS property used, it works only on Mac OS X.

## Extension Settings

None so far.

## Known Issues

VSCode is smart enough to recognize that the extension tampered its core files, so it will show a message box the first time, and "[Unsupported]" in the title bar.

## Release Notes

### 0.0.3
Forked from ZER0/roughify, with the intention of making a greyscale-antialiasing variant. Added CSS that will also apply to the Integrated Terminal and to the line numbers in the main editor gutter.

### 0.0.2

Initial release.
