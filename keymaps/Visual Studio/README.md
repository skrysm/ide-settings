# Visual Studio Keymap

## Export

1.  Export key bindings
1.  Re-import key bindings
1.  Export key bindings again (VS reorders the XML when importing so we to do steps 2 and 3 to get a consistent file)
1.  Use Visual Studio Code to format the file (via `Ctrl+Shift+P` and then `Format Document`).

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

## Recreating the Key Bindings

When switching to a new Visual Studio version (e.g. 2017 to 2019) you may wish to recreate the key bindings from scratch rather than importing them from the previous Visual Studio version.

The following tables list the key binding names as they appear in Visual Studio ("(default)" here means that the key binding has the correct value out-of-the-box).

The underlying keymap is: **Visual C# 2005**

**Notes:**

*   **For every key binding:** Always check the "Shortcut currently used by" drop down for *every* key binding and remove all other conflicting key bindings.
*   As "Scope" we use "Global" everywhere - unless the keybinding must be restricted to a certain scope. This way we make sure that the keybindings don't have other meaning in other parts of Visual Studio.
*   Keybindings with scope "Text Editor" are applied to every text editor (including XAML, XML, HTML...). So there's no need to define the same keybindings for different text editor types.

### General

| Function                          | Key Binding Name                                  | Scope
| ----------------------------------| ------------------------------------------------- | -----
| IDE Settings                      | `Tools.Options`                                   | Global
| ReSharper Settings Layers         | `ReSharper.ReSharper_ShowSettingsLayersDialog`    | Global
| New File in Current Directory     | `ReSharper.ReSharper_GenerateFileBesides`         | Global
| New Folder (in Sidebar)           | `ReSharper.ReSharper_GenerateNewFolder`           | Solution Explorer
| Open File                         | `File.OpenFile`                                   | Global
| Save All                          | (default)
| Go to Action/Command              | `Window.ActivateQuickLaunch` (VS2017), `Window.QuickLaunch` (VS2019) | Global
| Open File in Explorer             | `File.OpenContainingFolder`                       | Global
| Open File in Explorer             | `ProjectandSolutionContextMenus.Project.OpenFolderinFileExplorer` | Solution Explorer
| Locate Current File in Sidebar    | (default)
| Zoom In/Out                       | `View.ZoomIn`, `View.ZoomOut`                     | (Remove)

### Windows / Tabs

| Function                  | Key Binding Name              | Scope
| ------------------------- | ----------------------------- | -----
| Close Current Tab         | `Window.CloseDocumentWindow`  | Global
| Close All Tabs            | `Window.CloseAllDocuments`    | Global
| Close Other Tabs          | `File.CloseAllButThis`        | Global
| Go to Previous Editor Tab | `Window.PreviousTab`          | Global
| Go to Next Editor Tab     | `Window.NextTab`              | Global

### Search / Replace

| Function          | Key Binding Name                  | Scope
| ----------------- | --------------------------------- | -----
| Find Next         | (default)
| Find Previous     | (default)
| Search Everywhere | `ReSharper.ReSharper_GotoText`    | Global

### Editing

| Function                                  | Key Binding Name                          | Scope
| ----------------------------------------- | ----------------------------------------- | -----
| Quick Fix                                 | (default)
| Show Parameter Info                       | `ReSharper.ReSharper_ParameterInfoShow`   | Global
| Quick Documentation                       | (default)
| Refactor this                             | (default)
| Rename (Refactoring)                      | (default)
| Surround with                             | (default)
| Override Methods                          | `ReSharper_GenerateOverrides`             | Global
| Toggle Line Comment                       | `ReSharper.ReSharper_LineComment`         | Global
| Toggle Block Comment                      | `ReSharper.ReSharper_BlockComment`        | Global
| Cleanup File (with Profile Selection)     | (default)
| Cleanup File (with Default Profile)       | (default)
| Expand Selection                          | `ReSharper.ReSharper_ExtendSelection`     | Global
| Shrink Selection                          | `ReSharper.ReSharper_ShrinkSelection`     | Global
| Go to Previous Hump                       | `ReSharper_HumpPrev`                      | Global
| Go to Next Hump                           | `ReSharper_HumpNext`                      | Global
| Extend Selection to Previous Hump         | `ReSharper_HumpPrevExtend`                | Global
| Extend Selection to Next Hump             | `ReSharper_HumpNextExtend`                | Global
| Block Selection                           | (default)

**Note:** For "Toggle Comment" we still use the ReSharper functionality in VS2019, as the VS2019 functionality doesn't work, for example, in XAML.

### Navigation

| Function                                  | Key Binding Name
| ----------------------------------------- | ----------------
| Search Everything/Search for Symbol       | (default)
| Navigate to File                          | (default)
| Go to Implementation                      | (default)
| Find Usages                               | (default)
| Go to Member                              | (default)
| Go to Child Implementation (Interface)    | (default)
| Go to Parent Implementation (Interface)   | (default)
| Go to Previous Annotation                 | (default)
| Go to Next Annotation                     | (default)
| Navigate Back                             | (default)
| Navigate Forward                          | (default)
| Go to Line                                | (default)

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
