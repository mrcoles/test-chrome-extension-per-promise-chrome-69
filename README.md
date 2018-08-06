# Regression: User gesture error inside Promise Chain

In Chrome v70 (Canary), a previously working Promise chain inside an onclick handler is now encountering the following error while requesting the "downloads" permission:

> This function must be called during a user gesture permission

Currently running Chrome 67.0.3396.99, I am not seeing this error. Both were tested on Mac OSX 10.13.5. There is also a report of it happening in Chrome 69.0.3497 on Mac OS X 10.13.4.

I have reduced this example to the following popup.js code in this repo. Click on the popup icon to activate the extension and then click the link in the popup to see the result.
