# Zen Browser - macOS Traffic Lights Window Controls

This custom CSS theme replaces the standard Windows/Linux window control buttons (Close, Minimize, Maximize) in Zen Browser with the aesthetic macOS "Traffic Light" buttons.
!assets/custom-window.png
## 🎨 Features

- **macOS Styling**: Replaces square buttons with the iconic Red, Yellow, and Green circles.
- **Hover Effects**: Symbols (×, -, ⤢) only appear when you hover over the buttons, keeping the interface clean.
- **Smooth Animations**: Includes transition effects for opacity and background color changes.
- **Retina Ready**: Uses CSS shapes and system fonts, ensuring they look crisp on any display scaling.

## 🛠️ Installation

Zen Browser is based on Firefox, so it uses the standard ```userChrome.css``` method for UI customization.

### 🔍 Step 1: Locate your Profile Folder
1. Open **Zen Browser**.
2. Type ```about:support``` in the address bar and press Enter.
3. Look for the "**Profile Folder**" row in the "Application Basics" table.
4. Click the "**Open Folder**" (or "Show in Finder" on macOS) button.

## 📁Step 2: Create the Chrome Directory

1. Inside your profile folder, look for a folder named ```chrome```.
2. **If it doesn't exist**, create a new folder and name it ```chrome``` (all lowercase).

## ⚙️Step 3: Install the CSS

1. Take the ```chrome.css``` file above.
2. Rename it to ```userChrome.css```. (This is required for the browser to detect it).
3. Move this ```userChrome.css``` file into the ```chrome``` folder you opened in Step 2.
+ Path should look like: ```.../YourProfile/chrome/userChrome.css```

## ✅ Step 4: Enable Custom Styles (If not already enabled)

Zen Browser usually allows this by default, but if it doesn't work:
Type ```about:config``` in the address bar and press **Enter**.
Click "Accept the Risk and Continue".
Search for: ```toolkit.legacyUserProfileCustomizations.stylesheets```
Double-click it to set it to ```true```.

## 🚀Step 5: Restart

1. Close Zen Browser completely.
2. Re-open it to see your new traffic light buttons!

## 🔧 Customization

If you want to adjust the spacing or alignment, open the ```userChrome.css``` file in any text editor:
. **Adjust Spacing**: Find ```.titlebar-buttonbox``` and change ```gap: 10px;``` to a larger or smaller number.
. **Adjust Size**: Find ```.titlebar-button``` and change ```width: 14px;``` and ```height: 14px;``` to your preferred size.

## ⚠️ Troubleshooting

. **Buttons look cut off?** You may need to increase the ```padding``` in the ```.titlebar-buttonbox``` section.
. **Not showing up?* Ensure the file is named exactly ```userChrome.css``` (case-sensitive) and is inside the ```chrome``` folder.
