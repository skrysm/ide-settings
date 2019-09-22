# Visual Studio 2017 Key Bindings

## Export

1. Export key bindings
1. Re-import key bindings
1. Export key bindings again (VS reorders the XML when importing so we to do steps 2 and 3 to get a consistent file)
1. Use Visual Studio Code to format the file (via `Ctrl+Shift+P` and then `Format Document`).

## Exporting Key Bindings

Go to:

    Tools -> Import and Export Settings... -> Export selected environment settings

Then deselect `All Settings` and select:

    Options -> Environment -> Keyboard

Then export.

## Importing Key Bindings

Go to:

    Tools -> Import and Export Settings... -> Import selected environment settings

Say `No, just import new settings` and follow import wizard.
