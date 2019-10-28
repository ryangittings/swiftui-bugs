# SwiftUI Issues, Limitations & Unknowns
With Apple's documentation for SwiftUI being limited, I wanted to create a central resource of all bugs, issues and limitations with SwiftUI.

## Current Issues
- Context menu not showing on a custom view
- Environment/observed objects lose data on list view change
  - 🔨 **[Example](https://github.com/mecid/swiftui-bug)**
- Tab view resets view and navigation stack
  - 🔨 **[Example](https://github.com/pedrommcarrasco/swiftui-tabviewResetsViewsAndNavigationStack)**
- Modal views/sheets don't automatically have environment data
  - 🔨 **[Example](https://forums.developer.apple.com/thread/117651)**
- Scrollview with HStack and items have poor performance for large data sets (all child views are loaded on init).

## Limitations/Unknowns
- Unable to remove or customise list separators
- Unable to change navigation appearance for a single view
- Unable to easily support deep linking for universal links or notifications
- Unable to use a UISearchController with a SwiftUI view
  - 🔨 **[Example](https://stackoverflow.com/questions/58511758/swiftui-uisearchcontroller-searchresultscontroller-navigation-stack-issue)**
- Unable to remove a list item background altogether for one cell

Please feel free to PR and submit examples, workarounds and/or fixes so I can keep this up to date.
