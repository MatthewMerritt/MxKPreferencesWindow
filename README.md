# MMPreferencesWindow

## Example

To run the example project, clone the repo and open the project.

## Requirements

Minimum Requirements

Swift 5.0
Xcode 12
Installation

## Install with Swift Package Manager

Add the URL of this repository to your Xcode 11+ Project.
```
https://github.com/MatthewMerritt/MxKPreferencesWindow.git
```

## Usage

Create a NIB view for the settings you want, also create a NSView subclass that will be associated with the prefences view. Ensure they naming, add IBOutlets and IBActions. Next setup your main Storyboard or NIB menus call a IBAction to display your preferences.


```
    import MxKPreferencesWindow
    
    let preferencesWindowController: MxKPreferencesWindowController = MxKPreferencesWindowController.shared
    
    preferencesWindowController.addPreferenceView(title: "General", icon: "NSPreferencesGeneral", className: "MMPreferencesViewController", identifier: "GeneralView", nib: "GeneralView")

    @IBAction func preferencesButtonAction(_ sender: Any) {
        preferencesWindowController.showWindow (nil)
    }


## Author

MatthewMerritt, matthew.merritt@yahoo.com

## License

MxKPreferencesWindow is available under the MIT license. See the LICENSE file for more info.
