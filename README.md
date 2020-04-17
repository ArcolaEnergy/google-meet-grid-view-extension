# Introduction and acknowledgements

This extension shows everyone in a Google Meet. 

This version is a fork of the [St. George's Episcopal School, New Orleans, Louisiana version](https://github.com/stgeorgesepiscopal/google-meet-grid-view-extension) ([Chrome WebStore link](https://chrome.google.com/webstore/detail/google-meet-grid-view/bjkegbgpfgpikgkfidhcihhiflbjgfic)), with minimal changes. The purpose of this fork is to control the version deployed for [Arcola Energy](https://www.arcolaenergy.com/). You probably want the St. George's version, unless you are working for Arcola Energy, and you should use the Chrome WebStore link to install it.

The St. George's extension is "based almost entirely on [Chris Gamble's Userscript](https://greasyfork.org/en/scripts/397862-google-meet-grid-view), just packaged as a proper Chrome Extension so that we can push it via GAdmin to our faculty and students."

No data is stored by the extension, it's a purely cosmetic script. No extra permissions are required except access to meet.google.com. You can view all source code on the [public repository](https://github.com/stgeorgesepiscopal/google-meet-grid-view-extension).

If you feel both grateful and generous, feel free to visit the [St. George's donation page](https://www.stgnola.org/giving/make-a-donation) and make a gift using the form on the left side of the page. They say (in [the original README](https://github.com/stgeorgesepiscopal/google-meet-grid-view-extension/blob/master/README.md)): "This is a very trying time for our school, and I'm proud to say we're doing the right thing by paying all of our hourly wage-earners, even though they can't come into work and we don't have the revenue we typically would to do it with. So every little bit helps! Please use the Designation of "Other: Tech Team Support of StG Community Fund" "

# Cloning / building

This repo uses submodules to keep pulling the latest userscript (basically, I'm just injecting his script)

So instead of just `git clone` you'll want to do `git clone --recursive` if you're installing the script locally.

To build the script yourself, just clone the repo, go to the directory and use `zip -r chrome-extension.zip src` that will generate the zip file that you can upload to the Chrome Web Store (It costs $5 one time to become a developer on there, you can publish extensions as "unlisted" sdo you need the link to find them, but you have to publish it to make it available to anyone other than installing it from a directory in developer mode). The screenshot.jpg is taken from the original Chrome WebStore listing, but is included because one is required to publish it.

Be sure to adjust the variables in `manifest.json` to reflect your own information.
