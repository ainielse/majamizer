# majamizer
Region plug-in to clone an APEX session when opening in a new tab

After installing the plug-in, please review the help and comments contained in the plug-in.

You can use either the plug-in or the application process. You do not need both. **In both cases, use a server side condition so that it does not run on the login page.** It won't cause a big issue if it runs on the login page, but it will cause an unnecessary redirect on that page.

Note: this plug-in (or code) handles applications that use Session State Protection (SSP - Checksums in the URL). This can be greatly simplified if you application does not use SSP.

## Known Issues

1. Currently does NOT work for friendly URLs.
2. Special characters passed on the URL may cause a checksum error when the page reloads. It is best to only pass numbers on the URL. Strings without special characters will work, though.
