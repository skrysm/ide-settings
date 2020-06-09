# Visual Studio and ReSharper Settings

These are my personal settings for Visual Studio and ReSharper.

## Recommended Visual Studio Extensions

Recommended extension (besides ReSharper):

* [Solution Error Visualizer](https://marketplace.visualstudio.com/items?itemName=VisualStudioPlatformTeam.SolutionErrorVisualizer)
* [Trailing Whitespace Visualizer](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.TrailingWhitespaceVisualizer)
* [Fix Mixed Tabs](https://marketplace.visualstudio.com/items?itemName=VisualStudioPlatformTeam.FixMixedTabs)
* Disable Mouse Wheel Zoom
   * (For VS2017) [Disable Mouse Wheel Zoom](https://marketplace.visualstudio.com/items?itemName=NoahRichards.DisableMouseWheelZoom)
   * (For VS2019) [Disable Mouse Wheel Zoom for Visual Studio 2019](https://marketplace.visualstudio.com/items?itemName=reduckted.DisableMouseWheelZoom)
* [Disable Solution Explorer's Dynamic Nodes](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.DisableSolutionExplorersDynamicNodes)
   * Afterwards in VS click: `View` -> `Disable Solution Explorer's Dynamic Nodes`
* [Double-Click Maximize](https://marketplace.visualstudio.com/items?itemName=VisualStudioPlatformTeam.Double-ClickMaximize)

## Visual Studio Settings

Via `Tools` -> `Options...`:

* Environment
   * Import and Export Settings
      * Select appropriate folder for auto-save (file name: `CurrentSettings`)
   * Tabs and Windows
      * Check "Show pinned tabs on a separate row"
   * Trailing Whitespace (from extension)
      * Remove `.md` and `.markdown` from "Ignore pattern"
* Projects and Solutions
   * General
      * Check "Show output window when build starts"
* Source Control
   * Visual Studio Team Foundation Server
      * Uncheck "Resolve associated work items on check-in"
* Text Editor
   * General
      * Uncheck "Drag and drop text editing"
   * Advanced
      * Check "Show the difference overview margin" (for when comparing files in VS)
   * All Languages
      * General
         * Check "Line Numbers"
         * Uncheck "Apply Cut or Copy to blank lines when there is no selection"
      * CodeLense
         * Uncheck "Enable CodeLense"
* Debugging
   * General
      * Uncheck "Step over properties and operators"
* NuGet Package Manager
   * General
      * "Default package management format": "PackageReference"
* XAML Designer
   * Uncheck "Enable XAML Designer"

Via `Tools` -> `Customize...` (VS2019 or newer):

* Extensions Menu
   * Uncheck "ReSharper" (this way, the ReSharper menu again appears in the VS menu bar directly)


## Migrating Window Layout from older Visual Studio Version

First export all settings in the *old* Visual Studio to a *temporary* file.

Then edit this file and change `<ApplicationIdentity version="xx.x"/>` to the new Visual Studio version (see [here](https://stackoverflow.com/q/21996197/614177) for details):

* VS2017: 15.0
* VS2019: 16.0

Then import the following settings in the *new* Visual Studio:

* General Settings
   * Window Layouts

*Note:* The layout of ReSharper windows may not migrate this way.

## Import Key Bindings

For key bindings, see: <https://github.com/skrysmanski/ide-keymaps>

## ReSharper Settings

This repo contains the file `EditorSettings.DotSettings` which should be used at the "Computer Level".

This file only contains editor related setting. It explicitly does *not* contain any code style settings.
