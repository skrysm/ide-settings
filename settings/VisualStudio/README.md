# Visual Studio and ReSharper Settings

These are my personal settings for Visual Studio and ReSharper.

## Recommended Visual Studio Extensions

Recommended extension (besides [ReSharper](https://www.jetbrains.com/resharper/)):

* [Solution Error Visualizer](https://marketplace.visualstudio.com/items?itemName=VisualStudioPlatformTeam.SolutionErrorVisualizer)
* [Trailing Whitespace Visualizer](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.TrailingWhitespaceVisualizer)
* [Fix Mixed Tabs](https://marketplace.visualstudio.com/items?itemName=VisualStudioPlatformTeam.FixMixedTabs)
* [Disable Solution Explorer's Dynamic Nodes](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.DisableSolutionExplorersDynamicNodes)
  * Afterwards in VS click: `View` -> `Disable Solution Explorer's Dynamic Nodes`
* [Double-Click Maximize](https://marketplace.visualstudio.com/items?itemName=VisualStudioPlatformTeam.Double-ClickMaximize)
* [Output enhancer](https://marketplace.visualstudio.com/items?itemName=NikolayBalakin.Outputenhancer)
* [Tweaks](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.Tweaks)
* [FileIcons](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.FileIcons)

Uninstall/disable the following extensions:

* Visual Studio IntelliCode (VS2022): This sometimes conflicts with ReSharper's auto completion (inserting code you don't want to be inserted).

## Visual Studio Settings

Via `Tools` -> `Options...`:

* Environment
  * Accounts
    * Uncheck "Synchronize settings across devices when signed into Visual Studio" (see below for explanation)
  * Import and Export Settings
    * Select appropriate folder for auto-save (file name: `CurrentSettings`)
  * Tabs and Windows
    * Check "Colorize document tabs by project" (VS2022+)
    * Check "Show pinned tabs on a separate row"
  * Trailing Whitespace (from extension)
    * Remove `.md` and `.markdown` from "Ignore pattern"
  * Tweaks
    * Copy on Empty Selection: False
    * Enable Collapsing Attributes: False
* Projects and Solutions
  * General
    * Check "Show output window when build starts"
* Source Control
  * If *TFS* is used:
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
    * Scroll Bars
      * Check "Use bar mode for vertical scroll bar"
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

### Visual Studio Settings Synchronization

Visual Studio's handling of its settings has always been bad (in my opinion).

The main problem (as far as I understand it) is that Visual Studio does *not* save its settings when you hit the "Ok" button in the settings dialog but when you close Visual Studio. Also, it *always* saves *all* of its settings - even if no settings have been changed. And since settings are *not* synchronized between running Visual Studio instances, you can make settings changes in one instance but effectively lose them if you don't close *that* instance last.

This effect is "amplified" when enabling Visual Studio's settings synchronization because you now not only need to consider the Visual Studio instances on your *current* machine - but **on all machines** you have Visual Studio running. So, the last instance on all of your machines "wins".

In my trial of this feature I managed to **lose all of my settings** in just 5 minutes (because settings synchronization is enabled on *fresh* Visual Studio installations).

So, my conclusion is:

> Do **not** use Visual Studio settings synchronization!

As a side note: The synchronized settings are not versioned (in Git or something similar, like for example in IntelliJ's settings sync functionality). So you can *not* easily recover from losing all your settings by simply going to an older revision/commit.

## Recreating Window Layouts

The window layouts can be found in the two `window-layout-...png` files (for reference). Simply recreate them in Visual Studio.

![regular layout](window-layout-regular.png)

![debug layout](window-layout-debug.png)

## Importing Key Bindings

For key bindings, see [keymaps](../../keymaps/VisualStudio/README.md).

## ReSharper Settings

This repo contains the file `EditorSettings.DotSettings` which should be used at the "Computer Level".

This file only contains editor related setting. It explicitly does *not* contain any code style settings.
