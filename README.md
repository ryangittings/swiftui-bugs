# SwiftUI Issues, Limitations & Unknowns
With Apple's documentation for SwiftUI being limited, I wanted to create a central resource of all bugs, issues and limitations with SwiftUI.

## Current Issues
- Context menu not showing on a custom view
- Environment/observed objects lose data on list view change. This problem appear in case when parent view updated with same data in terms of hash. The bug is not appearing when the parent view updated with different data.
  - 🔨 **[Example](https://github.com/mecid/swiftui-bug)**
- Tab view resets view and navigation stack
  - 🔨 **[Example](https://github.com/pedrommcarrasco/swiftui-tabviewResetsViewsAndNavigationStack)**
- Modal views/sheets don't automatically have environment data
  - 🔨 **[Example](https://forums.developer.apple.com/thread/117651)**
- Scrollview with HStack and items have poor performance for large data sets (all child views are loaded on init).
- Multiple buttons in a list row causes both buttons to be actioned upon when tapped
  - 🔨 **[Example](https://stackoverflow.com/questions/56561064/swiftui-multiple-buttons-in-a-list-row)**
  - ↪️ **[Workaround](https://stackoverflow.com/a/56561423/11651357)**
- 'Tried to pop to a view controller that doesn't exist' crash 
  - 🔨 **[Example](https://stackoverflow.com/q/58404725/11651357)**
  - ↪️ **[Workaround](https://stackoverflow.com/a/58466670/11651357)**

## Limitations/Unknowns
- No SwiftUI equivalent to UICollectionView
- Unable to remove or customise list separators
- Unable to change navigation appearance for a single view
- Unable to easily support deep linking for universal links or notifications
- Unable to use a UISearchController with a SwiftUI view
  - 🔨 **[Example](https://stackoverflow.com/questions/58511758/swiftui-uisearchcontroller-searchresultscontroller-navigation-stack-issue)**
- Unable to remove a list item background altogether for one cell
- Unable to know when view becomes active again (equivalent to viewDidAppear)

Please feel free to PR and submit examples, workarounds and/or fixes so I can keep this up to date.
