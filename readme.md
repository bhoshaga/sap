# Project Title

Binary releases for SAP2000

## Description

The releases were generated via:

```
npm run dist:win
```

The releases are created in "Draft" mode and will need to be manually set to "Release" before being available for auto update by clients.

## Prevent auto generation of releases

In package.json, remove these lines (which are located just above "build"):

```
  "repository": "https://github.com/bhoshaga/sap",
  "publish": {
    "provider": "GitHub"
  },
```
Note that, removing the above, will prompt npm to spew harmless warnings. That's fine as the binaries will still be generated in "dist".

Add them back in when you want resume auto generation of releases.
