
# Brandperity

## Version 0.1

<!--<img src="./demo.gif" width=600></img>-->

Brandperity is the working title for a Google Chrome extension that allows you to personalise the Acme tenant to deliver a custom demo. It works by modifying text, images, and Material icons in the Acme UI, by applying substitutions locally in your browser. 

## 🎉 Current Features 🎉
- [x] Works in Chrome & Brave
- [x] Templates for verticals
- [x] Customise data sources
- [x] Customise Customer 360 attributes & tables
- [x] Change Segment/ Query Editor attributes
- [x] Build segments using customised attribute names 
- [x] Change charts and labels on the Segment Insights tab
- [x] Change destination names and labels

## ⌛ Coming Soon ⌛
- [x] Change icons in the Customer 360 screens
- [x] Better system for managing logos
- [x] Streamlined import/ export of personalisations
- [x] Better templatized examples
- [x] Overhaul of the extension's UI
- [x] Better save/load/import/export list options
- [x] Ability to easily share configurations
- [x] Manage configurations in Google Sheets!!

## 🐛 Known Bugs! 🐛

- [x] Switching between C360 databases will reset the view of attributes back to the default. Exit the C360 tab and re-enter it to reset this.
- [x] Values containing - or + (Both as the string you want to replace and the one you are replacing with)can cause problems like <undefined> to appear in the UI or substituions not to be made correctly. Currently no workaround, but I know why this happens. Please test carefully until fixed in the next release.
- [x] Any refreshes performed on Segment pages sometimes lead to the UI becoming stuck as it reloads. This only happens when refrehsing, and not when navigating normally as per a demo.
- [x] Clearing a list and importing a new, shorter one will cause the console.log to fill with errors in an infinite loop. (Does not impact the user experience). This is due to lazy coding and will be fixed in the next release.
- [x] Sometimes (and always on the first use after a fresh install) the 'save' button appears not to work/ your list will disappear or not look updated. Also the 'refresh' button seems to break at the same time. If this happens, refresh the page and open the extension again - your changes should all be reflected.


## Install

*As this is still an early release, Brandperity is not yet packaged up (Google requires packaged extensions are released through the Chome Web Store), so a few manual steps are required to install* 

- Click the green 'Code' button near the top of this page
- From the dropdown, click 'Download ZIP'
- Move the Zip file to a folder on your local machine & unpack
- Go to your favourite browser (Chrome or Brave)
- In the address bar type `chrome://extensions`
- On the right hand side of the window make sure 'Developer Mode' is enabled
- Click 'Load Unpacked'
- Navigate to the directory containing your unpacked zip file
- Navigate to the 'dist' directory and click 'Select' 
- Close the extensions window
- Still in Chrome/ Brave, click the puzzle piece icon and click the pin next to the Brandperity extension. This puts the icon next to the address bar in your browser
- Navigate to Acme in Amperity
- Click the Brandperity icon and follow instructions 
