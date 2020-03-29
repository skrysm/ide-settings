# Visual Studio/ReSharper based Key Maps

This repository contains key maps for various IDEs that make them work like Visual Studio with ReSharper installed. (This way I don't need to remember different shortcuts with each IDE ;P )

## Key Bindings

### General

| Function                          | Key Binding               | VSCode | VS | IntelliJ
| --------------------------------- | ------------------------- | ------ | -- | --------
| IDE Settings                      | `Ctrl + ,`                | ✓ | ✓ | ✓
| ReSharper Settings Layers         | `Ctrl + Shift + ,`        | × | ✓ | ×
| New File in Current Directory     | `Ctrl + N`                | ✓ | ✓ | ✓
| New Folder (in Sidebar)           | `Ctrl + Shift + N`        | ✓ | ✓ | ✓
| Open File                         | `Ctrl + O`                | ✓ | ✓ | ✓
| Save All                          | `Ctrl + Shift + S`        | ✓ | ✓ | ✓
| Go to Action/Command              | `Ctrl + Shift + A`        | ✓ | ✓ | ✓
| Open File in Explorer [1]         | `Alt + Shift + R`         | ✓ | ✓ | ✓
| Locate Current File in Sidebar    | `Alt + Shift + L`         | ✓ | ✓ | ✓
| Zoom In/Out                       | - (removed key bindings)  | ✓ | ✓ | ✓

*Footnotes:*

1.  Both in editor and project explorer sidebar.

### Windows / Tabs

| Function                  | Key Binding               | VSCode | VS | IntelliJ
| ------------------------- | ------------------------- | ------ | -- | --------
| Close All Windows         | `Ctrl + Shift + W`        | ✓ | ✓ | ✓
| Close Other Windows       | `Ctrl + Shift + Alt + W`  | ✓ | ✓ | ✓
| Go to Previous Editor Tab | `Ctrl + PageUp`           | ✓ | ✓ | ✓
| Go to Next Editor Tab     | `Ctrl + PageDown`         | ✓ | ✓ | ✓

### Search / Replace

| Function          | Key Binding           | VSCode | VS | IntelliJ
| ----------------- | --------------------- | ------ | -- | --------
| Find Next         | `F3`                  | ✓ | ✓ | ✓
| Find Previous     | `Shift + F3`          | ✓ | ✓ | ✓
| Search Everywhere | `Ctrl + Shift + F`    | ✓ | ✓ | ✓

### Editing

| Function                                  | Key Binding               | VSCode | VS | IntelliJ
| ----------------------------------------- | ------------------------- | ------ | -- | --------
| Quick Fix                                 | `Alt + Enter`             | ✓ | ✓ | ✓
| Show Parameter Info                       | `Ctrl + P`                | × | ✓ | ✓
| Quick Documentation                       | `Ctrl + Shift + F1`       | × | ✓ | ✓
| Refactor this                             | `Ctrl + Shift + R`        | × | ✓ | ✓
| Rename (Refactoring)                      | `Ctrl + R, Ctrl + R`      | ✓ | ✓ | ✓
| Surround with                             | `Ctrl + E, U`             | × | ✓ | ✓
| Override Methods                          | `Ctrl + Shift + O`        | × | ✓ | ✓
| Toggle Line Comment                       | `Ctrl + Shift + 7`        | ✓ | ✓ | ✓
| Toggle Block Comment                      | `Ctrl + Shift + Alt + 7`  | ✓ | ✓ | ✓
| Cleanup File (with Profile Selection)     | `Ctrl + E, C`             | × | ✓ | ✓
| Cleanup File (with Default Profile)       | `Ctrl + E, F`             | × | ✓ | ✓
| Expand Selection                          | `Alt + Shift + Up`        | ✓ | ✓ | ✓
| Shrink Selection                          | `Alt + Shift + Down`      | ✓ | ✓ | ✓
| Go to Previous Hump                       | `Alt + Left`              | ✓ | ✓ | ✓
| Go to Next Hump                           | `Alt + Right`             | ✓ | ✓ | ✓
| Extend Selection to Previous Hump         | `Alt + Shift + Left`      | ✓ | ✓ | ✓
| Extend Selection to Next Hump             | `Alt + Shift + Right`     | ✓ | ✓ | ✓
| Block Selection                           | `Alt` + Mouse             | × | ✓ | ✓
| Block Selection                           | Middle Mouse Button       | ✓ | × | ✓

### Navigation

| Function                                  | Key Binding           | VSCode | VS | IntelliJ
| ----------------------------------------- | --------------------- | ------ | -- | --------
| Search Everything/Search for Symbol       | `Ctrl + T`            | ✓ | ✓ | ✓
| Navigate to File                          | `Ctrl + Shift + T`    | ✓ | ✓ | ✓
| Go To Implementation                      | `F12`                 | ✓ | ✓ | ✓
| Find Usages                               | `Shift + F12`         | ✓ | ✓ | ✓
| Go to Member                              | `Alt + ß`             | × | ✓ | ✓
| Go to Child Implementation (Interface)    | `Alt + End`           | × | ✓ | ✓
| Go to Parent Implementation (Interface)   | `Alt + Home`          | × | ✓ | ✓
| Go to Previous Annotation                 | `Alt + PgUp`          | ✓ | ✓ | ✓
| Go to Next Annotation                     | `Alt + PgDown`        | ✓ | ✓ | ✓
| Navigate Back                             | `Ctrl + -`            | ✓ | ✓ | ✓
| Navigate Forward                          | `Ctrl + Shift + -`    | ✓ | ✓ | ✓
| Go to Line                                | `Ctrl + G`            | ✓ | ✓ | ✓

### Running / Debugging

| Function              | Key Binding   | VSCode | VS | IntelliJ
| --------------------- | ------------- | ------ | -- | --------
| Toggle Breakpoint     | `F9`          | ✓ | ✓ | ✓
| Run in Debugger       | `F5`          | ✓ | ✓ | ✓
| Run without Debugger  | `Ctrl + F5`   | ✓ | ✓ | ✓
| Resume/Continue       | `F5`          | ✓ | ✓ | ✓
| Step Into             | `F11`         | ✓ | ✓ | ✓
| Step Out              | `Shift + F11` | ✓ | ✓ | ✓
| Step Over             | `F10`         | ✓ | ✓ | ✓
