# Visual Studio-/ReSharper-based Keymap

This directory contains a keymap for various IDEs that make them work like Visual Studio with ReSharper installed.

## Keybindings

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
| Refresh TFS information [2]       | `Ctrl + Shift + F5`       | × | ✓ | ×

*Footnotes:*

1. Both in editor and project explorer sidebar.
1. Only required for Visual Studio and TFS.

### Windows / Tabs

| Function                              | Key Binding               | VSCode | VS | IntelliJ
| ------------------------------------- | ------------------------- | ------ | -- | --------
| Close Current Tab                     | `Ctrl + W`                | ✓ | ✓ | ✓
| Close All Tabs                        | `Ctrl + Shift + W`        | ✓ | ✓ | ✓
| Close Other Tabs                      | `Ctrl + Shift + Alt + W`  | ✓ | ✓ | ✓
| Go to Previous Editor Tab             | `Ctrl + PageUp`           | ✓ | ✓ | ✓
| Go to Next Editor Tab                 | `Ctrl + PageDown`         | ✓ | ✓ | ✓
| Show/Toggle Outline (File Structure)  | `Shift + Alt + O`         | × | ✓ |

### Search / Replace

| Function          | Key Binding           | VSCode | VS | IntelliJ
| ----------------- | --------------------- | ------ | -- | --------
| Find Next         | `F3`                  | ✓ | ✓ | ✓
| Find Previous     | `Shift + F3`          | ✓ | ✓ | ✓
| Search Everywhere | `Ctrl + Shift + F`    | ✓ | ✓ | ✓

### Editing

| Function                                  | Key Binding                           | VSCode | VS | IntelliJ
| ----------------------------------------- | ------------------------------------- | ------ | -- | --------
| Quick Fix                                 | `Alt + Enter`                         | ✓ | ✓ | ✓
| Show Parameter Info                       | `Ctrl + P`                            | × | ✓ | ✓
| Quick Documentation                       | `Ctrl + Shift + F1`                   | × | ✓ | ✓
| Refactor this                             | `Ctrl + Shift + R`                    | × | ✓ | ✓
| Rename (Refactoring)                      | `Ctrl + R, Ctrl + R` (`Ctrl+R, R`)    | ✓ | ✓ | ✓
| Surround with                             | `Ctrl + E, U` (`Ctrl + E, Ctrl + U`)  | × | ✓ | ✓
| Override Methods                          | `Ctrl + Shift + O`                    | × | ✓ | ✓
| Toggle Line Comment                       | `Ctrl + Shift + 7`                    | ✓ | ✓ | ✓
| Toggle Block Comment                      | `Ctrl + Shift + Alt + 7`              | ✓ | ✓ | ✓
| Cleanup File (with Profile Selection)     | `Ctrl + E, C` (`Ctrl + E, Ctrl + C`)  | × | ✓ | ✓
| Cleanup File (with Default Profile)       | `Ctrl + E, F` (`Ctrl + E, Ctrl + F`)  | × | ✓ | ✓
| Expand Selection                          | `Alt + Shift + Up`                    | ✓ | ✓ | ✓
| Shrink Selection                          | `Alt + Shift + Down`                  | ✓ | ✓ | ✓
| Go to Previous Hump                       | `Alt + Left`                          | ✓ | ✓ | ✓
| Go to Next Hump                           | `Alt + Right`                         | ✓ | ✓ | ✓
| Extend Selection to Previous Hump         | `Alt + Shift + Left`                  | ✓ | ✓ | ✓
| Extend Selection to Next Hump             | `Alt + Shift + Right`                 | ✓ | ✓ | ✓
| Block Selection                           | `Alt` + Mouse                         | × | ✓ | ✓
| Block Selection                           | Middle Mouse Button                   | ✓ | × | ✓
| Expand/Unfold all Regions                 | `Ctrl + M, L` (`Ctrl + M, Ctrl + L`)  | ✓ | ✓ | ✓

### Navigation

| Function                                  | Key Binding           | VSCode | VS | IntelliJ
| ----------------------------------------- | --------------------- | ------ | -- | --------
| Search Everything/Search for Symbol       | `Ctrl + T`            | ✓ | ✓ | ✓
| Navigate to File                          | `Ctrl + Shift + T`    | ✓ | ✓ | ✓
| Go To Implementation                      | `F12`                 | ✓ | ✓ | ✓
| Find Usages                               | `Shift + F12`         | ✓ | ✓ | ✓
| Go to Member                              | `Alt + ß`             | × | ✓ | ✓
| Go to Parent Implementation (Base)        | `Alt + Home`          | × | ✓ | ✓
| Go to Child Implementation (Inheritors)   | `Alt + End`           | × | ✓ | ✓
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
