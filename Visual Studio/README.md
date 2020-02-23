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

## Recreating the Key Bindings

When switching to a new Visual Studio version (e.g. 2017 to 2019) you may wish to recreate the key bindings from scratch rather than importing them from the previous Visual Studio version.

The following tables list the key binding names as they appear in Visual Studio ("(default)" here means that the key binding has the correct value out-of-the-box):

### General

| Function                                                          | Key Binding Name                  | Scope
| ----------------------------------------------------------------- | --------------------------------- | -----
| IDE Settings                                                      | `Tools.Options`                   | Global, Text Editor
| ReSharper Settings Layers                                         | `ReSharper.ReSharper_ShowSettingsLayersDialog` | Global, Text Editor
| Save All                                                          | (default)
| Search Everywhere                                                 | `ReSharper.ReSharper_GotoText`    | Global
| Find Next                                                         | (default)
| Find Previous                                                     | (default)
| Close All Windows                                                 | `Window.CloseAllDocuments`        | Global, Text Editor
| Close Other Windows                                               | `File.CloseAllButThis`            | Global, Text Editor
| Go To Previous Editor Tab                                         | `Window.PreviousTab`              | Global, Text Editor
| Go To Next Editor Tab                                             | `Window.NextTab`                  | Global, Text Editor
| Go to Action/Command                                              | `Window.ActivateQuickLaunch` (VS2017), `Window.QuickLaunch` (VS2019) | Global
| Open File in Explorer (both editor and project explorer sidebar)  | `File.OpenContainingFolder`       | Text Editor
| Open File in Explorer (both editor and project explorer sidebar)  | `ProjectandSolutionContextMenus.Project.OpenFolderinFileExplorer` | Solution Explorer
| Locate Current File in Sidebar                                    | (default)
| Zoom In/Out                                                       | `View.ZoomIn`, `View.ZoomOut`     | -

### Code Editing

| Function                                  | Key Binding Name                          | Scope
| ----------------------------------------- | ----------------------------------------- | -----
| Quick Fix                                 | (default)
| Search Everything/Search for Symbol       | (default)
| Open File                                 | (default)
| Go To Implementation                      | (default)
| Find Usages                               | (default)
| Go To Member                              | (default)
| Go To Child Implementation (Interface)    | (default)
| Go To Parent Implementation (Interface)   | (default)
| Go To Next Annotation                     | (default)
| Go To Previous Annotation                 | (default)
| Navigate Back                             | (default)
| Navigate Forward                          | (default)
| Go To Line                                | (default)
| Toggle Comment                            | `ReSharper.ReSharper_LineComment`         | Text Editor, XAML Designer
| Refactor this                             | (default)
| Rename (Refactoring)                      | (default)
| Surround with                             | (default)
| Expand Selection                          | `ReSharper.ReSharper_ExtendSelection`     | Text Editor
| Shrink Selection                          | `ReSharper.ReSharper_ShrinkSelection`     | Text Editor
| Go to Previous Hump                       | `ReSharper_HumpPrev`                      | Text Editor
| Go to Next Hump                           | `ReSharper_HumpNext`                      | Text Editor
| Extend Selection to Previous Hump         | `ReSharper_HumpPrevExtend`                | Text Editor
| Extend Selection to Next Hump             | `ReSharper_HumpNextExtend`                | Text Editor
| Block Selection                           | (default)
| Show Parameter Info                       | `ReSharper.ReSharper_ParameterInfoShow`   | Text Editor
| Quick Documentation                       | (default)
| Override Methods                          | `ReSharper_GenerateOverrides`             | Text Editor
| Cleanup File (with Profile Selection)     | (default)
| Cleanup File (with Default Profile)       | (default)

### Running and Debugging

| Function              | Key Binding Name
| --------------------- | ----------------
| Toggle Breakpoint     | (default)
| Run in Debugger       | (default)
| Run without Debugger  | (default)
| Resume/Continue       | (default)
| Step Into             | (default)
| Step Out              | (default)
| Step Over             | (default)
