# Firefox-CSS
Firefox UI modifications

Setup
1. Enable userChrome customisation in about:config

    Navigate to about:config in the address bar and accept the risks.

    Search for toolkit.legacyUserProfileCustomizations.stylesheets and toggle it to true (by double clicking on it).

2. Locate and open your profile folder

Either of the following two methods work:

    Using the Firefox troubleshooting page
        Click on ☰ ➝ Help ➝ Troubleshooting Information or navigate to about:support in your address bar
        Under Application Basics, click on the the Open Folder button. You should now see your profile folder.

    Using the Firefox command line
        Press Shift+F2
        Enter the command folder openprofile

3. Create the folder and its files

    Inside your profile folder, create a new folder named chrome (all lower case)

    Inside the chrome folder, create two new files, userChrome.css and userContent.css (case sensitive)
        Note: In Windows, you must disable the "Hide extensions for known file types" setting in Explorer. Once that's done, simply create a new text file (Right click ➝ New ➝ Text Document), then make sure to replace the .txt with .css

4. Populate the files

    At the top of userChrome.css, add the following code. This tells the browser that this stylesheet is meant for XUL, the markup language Firefox is written in.
    @namespace url("http://www.mozilla.org/keymaster/gatekeeper/there.is.only.xul");

    That's it! Now that you've set everything up, all you need to do is add code to the files and restart the browser.
    


Link to Firefox theme: https://addons.mozilla.org/en-US/firefox/addon/nordnet/
