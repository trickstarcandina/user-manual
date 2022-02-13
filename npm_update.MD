[This is the new best way to upgrade npm on Windows.](https://github.com/felixrieseberg/npm-windows-upgrade)

# Run PowerShell as Administrator
```
Set-ExecutionPolicy Unrestricted -Scope CurrentUser -Force
npm install -g npm-windows-upgrade
npm-windows-upgrade
```

Note: Do not run npm i -g npm. Instead use npm-windows-upgrade to update npm going forward. Also if you run the Node.js installer, it will replace the Node.js version.

- Upgrades npm in-place, where Node.js installed it.
- Easy updating, update to the latest by running npm-windows-upgrade -p -v latest.
- Does not modify the default path.
- Does not change the default global package location.
- Allows easy upgrades and downgrades.
- A list of versions matched between NPM and Node.js (https://nodejs.org/en/download/releases/) - but you will need to download the Node.js installer and run that to update Node.js (https://nodejs.org/en/)


https://stackoverflow.com/questions/18412129/how-can-i-update-npm-on-windows/27464115
