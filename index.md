
# Brandperity

## Version 0.1

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
- [x] Support for Regular Expressions, case insensitivity, 'Starts With', 'Ends With', 'Match Whole Word' etc.
- [x] 'Hide All Except...' Will hide the huge lists of segments and queries you see in the UI except for the ones you want for your demo.
- [x] Rewrite the main hacky substitution module, which currently works by looping around the page looking for changes until certain conditions are met, to a model that watches for DOM mutations using a more elegant JavaScript core library (MutationObserver). This will result in a smoother user experience and fewer visual bugs.

## 🐛 Known Bugs! 🐛

- [x] Switching between C360 databases will reset the view of attributes back to the default. Exit the C360 tab and re-enter it to reset this.
- [x] Values containing - or + (Both as the string you want to replace and the one you are replacing with) can cause problems like <undefined> to appear in the UI or substitutions not to be made correctly. Currently, there is no workaround, but I know why this happens. Please test carefully until it is fixed in the next release.
- [x] Any refreshes performed on Segment pages sometimes lead to the UI becoming stuck as it reloads. This only happens when refreshing, and not when navigating normally as per a demo.
- [x] Clearing a list and importing a new, shorter one will cause the console.log to fill with errors in an infinite loop. (Does not impact the user experience). This is due to lazy coding and will be fixed in the next release.
- [x] Sometimes (and always on the first use after a fresh install) the 'save' button appears not to work/ your list will disappear or not look updated. Also the 'refresh' button seems to break at the same time. If this happens, refresh the page and open the extension again - your changes should all be reflected.
- [x] If you have conflicting changes (i.e. you rename a certain field twice), you will see odd behaviour (sometimes) like values switching back and forth at very high speeds in the interface. As a workaround, remove these changes.
- [x] Clicking into a chart in Segment Insights will show the incorrect labels on the right-hand side
- [x] Sometimes, changing lots of values in a list without adding or deleting anything will cause the UI (or the extension) to look empty. If this happens, refresh both. No data should be lost.

## 👀 Things to watch out for! 👀

- [x] Searching for changed attributes will cause weirdness in the menu; don't do it in a demo!
- [x] If re-naming insight chart labels, bear in mind they are actually written as "Preferred Brand", not "PREFERRED BRAND" as they appear in the label. There is no case insensitivity at the moment, so you will not see your change work unless you case your change like the first example here
- [x] Weird word substitutions are common at the moment... Avoid changing terms like 'NY' and 'WA' as you will see words change to weird values. This isn't a bug, but due to not having very advanced substitution options yet.

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
