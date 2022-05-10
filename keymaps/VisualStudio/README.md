# Visual Studio Keymap

## Export

1. Export key bindings
1. Re-import key bindings
1. Export key bindings again (VS reorders the XML when importing so we to do steps 2 and 3 to get a consistent file)
1. Use Visual Studio Code to format the file (via `Ctrl + Shift + P` and then `Format Document`).

## Exporting Key Bindings

Go to:

    Tools -> Import and Export Settings... -> Export selected environment settings

Then deselect `All Settings` and select:

    Options -> Environment -> Keyboard

Then export.

## Importing Key Bindings

Optional: Tools -> Options -> Keyboard -> Reset

Go to:

    Tools -> Import and Export Settings... -> Import selected environment settings

Say `No, just import new settings` and follow import wizard.

## Recreating the Key Bindings from Scratch

When switching to a new Visual Studio version (e.g. 2017 to 2019) you may wish to recreate the key bindings from scratch rather than importing them from the previous Visual Studio version.

To start, follow the following steps:

1. Open the ReSharper settings (`Manage Options` -> `This computer`)
   1. `Keyboard` -> `Shortcut Scheme`
   1. Select `None` as Keyboard Scheme
   1. Confirm with `Save`
1. Open the Visual Studio settings
   1. `Environment` -> `Keyboard`
   1. Click `Reset`
   1. Select `Visual C# 2005` from the dropdown
   1. Click `OK`

The following tables list the key binding names as they appear in Visual Studio.

**Notes:**

* **For every key binding:** Always check the "Shortcut currently used by" drop down for *every* key binding and remove all other conflicting key bindings (only those with a different scope need to be removed explicitly).
* As "Scope" we use "Global" everywhere - unless the keybinding must be restricted to a certain scope. This way we make sure that the keybindings don't have other meaning in other parts of Visual Studio.
* Keybindings with scope "Text Editor" are applied to every text editor (including XAML, XML, HTML...). So there's no need to define the same keybindings for different text editor types.

### General

| Function                          | Key Binding Name                                                  | Scope
| ----------------------------------| ----------------------------------------------------------------- | -----
| IDE Settings                      | `Tools.Options`                                                   | Global
| ReSharper Settings Layers         | `ReSharper.ReSharper_ShowSettingsLayersDialog`                    | Global
| New File in Current Directory     | `ReSharper.ReSharper_GenerateFileBesides`                         | Global
| New Folder (in Sidebar)           | `ReSharper_GenerateNewFolder`                                     | Solution Explorer
| Open File                         | `File.OpenFile`                                                   | Global
| Save All                          | `File.SaveAll`                                                    | Global
| Go to Action/Command              | `Window.QuickLaunch`                                              | Global
| Open File in Explorer             | `File.OpenContainingFolder`                                       | Global
| Open File in Explorer             | `ProjectandSolutionContextMenus.Project.OpenFolderinFileExplorer` | Solution Explorer
| Locate Current File in Sidebar    | `ReSharper_LocateItemInSolutionOrAssemblyExplorer`                | Global
| Zoom In/Out                       | `View.ZoomIn`, `View.ZoomOut`                                     | (Remove)
| Refresh TFS information           | `File.TfsRefreshStatus`                                           | Team Explorer

### Windows / Tabs

| Function                              | Key Binding Name                                                  | Scope
| ------------------------------------- | ----------------------------------------------------------------- | -----
| Close Current Tab                     | `Window.CloseDocumentWindow`                                      | Global
| Close All Tabs                        | `Window.CloseAllDocuments`                                        | Global
| Close Other Tabs                      | `File.CloseAllButThis`                                            | Global
| Go to Previous Editor Tab             | `Window.PreviousTab` (remove binding  for all other commands!)    | Global
| Go to Next Editor Tab                 | `Window.NextTab` (remove binding  for all other commands!)        | Global
| Focus Project Sidebar                 | `View.SolutionExplorer`                                           | Global
| Show/Toggle Outline (File Structure)  | `ReSharper.ReSharper_ShowCodeStructure`                           | Global
| Jump back to editor (from sidebar)    | (default)

### Search / Replace

| Function          | Key Binding Name                  | Scope
| ----------------- | --------------------------------- | -----
| Find Next         | `Edit.FindNext`                   | Global
| Find Previous     | `Edit.FindPrevious`               | Global
| Search Everywhere | `ReSharper.ReSharper_GotoText`    | Global

### Editing

| Function                                  | Key Binding Name                          | Scope
| ----------------------------------------- | ----------------------------------------- | -----
| Quick Fix                                 | `ReSharper_AltEnter`                      | Text Editor
| Generate Code                             | `ReSharper.ReSharper_Generate`            | Text Editor
| Complete Statement                        | `ReSharper.ReSharper_CompleteStatement`   | Text Editor
| Show Parameter Info                       | `ReSharper.ReSharper_ParameterInfoShow`   | Text Editor
| Quick Documentation                       | `ReSharper.ReSharper_QuickDoc`            | Text Editor
| Refactor this                             | `ReSharper.ReSharper_RefactorThis`        | Global
| Rename (Refactoring)                      | `ReSharper.ReSharper_Rename`              | Global
| Surround with                             | `ReSharper.ReSharper_SurroundWith`        | Text Editor
| Override Methods                          | `ReSharper_GenerateOverrides`             | Text Editor
| Toggle Line Comment                       | `ReSharper.ReSharper_LineComment`         | Text Editor
| Toggle Block Comment                      | `ReSharper.ReSharper_BlockComment`        | Text Editor
| Cleanup File (with Profile Selection)     | `ReSharper.ReSharper_CleanupCode`         | Text Editor
| Cleanup File (with Default Profile)       | `ReSharper.ReSharper_SilentCleanupCode`   | Text Editor
| Expand Selection                          | `ReSharper.ReSharper_ExtendSelection`     | Text Editor
| Shrink Selection                          | `ReSharper.ReSharper_ShrinkSelection`     | Text Editor
| Go to Previous Hump                       | `ReSharper_HumpPrev`                      | Text Editor
| Go to Next Hump                           | `ReSharper_HumpNext`                      | Text Editor
| Extend Selection to Previous Hump         | `ReSharper_HumpPrevExtend`                | Text Editor
| Extend Selection to Next Hump             | `ReSharper_HumpNextExtend`                | Text Editor
| Block Selection                           | -
| Expand/Unfold all Regions                 | `Edit.ExpandAllOutlining`                 | Text Editor

**Note:** For "Toggle Comment" we still use the ReSharper functionality in VS2019, as the VS2019 functionality doesn't work, for example, in XAML.

### Navigation

| Function                                  | Key Binding Name                          | Scope
| ----------------------------------------- | ----------------------------------------- | -----
| Search Everything/Search for Symbol       | `ReSharper.ReSharper_GotoType`            | Global
| Navigate to File                          | `ReSharper.ReSharper_GotoFile`            | Global
| Go to Implementation                      | `Edit.GoToDefinition`                     | Text Editor
| Find Usages                               | `ReSharper.ReSharper_FindUsages`          | Text Editor
| Go to Member                              | `ReSharper.ReSharper_GotoFileMember`      | Text Editor
| Go to Parent Implementation (Base)        | `ReSharper.ReSharper_GotoBase`            | Text Editor
| Go to Child Implementation (Inheritors)   | `ReSharper.ReSharper_GotoInheritors`      | Text Editor
| Go to Previous Annotation/Issue           | `ReSharper.ReSharper_GotoPrevHighlight`   | Text Editor
| Go to Next Annotation/Issue               | `ReSharper.ReSharper_GotoNextHighlight`   | Text Editor
| Navigate Back                             | `View.NavigateBackward`                   | Global
| Navigate Forward                          | `View.NavigateForward`                    | Global
| Go to Line                                | `Edit.GoTo`                               | Global

### Running / Debugging

| Function              | Key Binding Name
| --------------------- | ----------------
| Toggle Breakpoint     | (default)
| Run in Debugger       | (default)
| Run without Debugger  | (default)
| Resume/Continue       | (default)
| Step Into             | (default)
| Step Out              | (default)
| Step Over             | (default)
