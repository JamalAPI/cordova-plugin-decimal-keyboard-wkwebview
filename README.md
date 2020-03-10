# cordova-plugin-decimal-keyboard-wkwebview
[![Linked In](https://img.shields.io/badge/Linked-In-blue.svg)](https://www.linkedin.com/in/john-i-doherty) [![Twitter Follow](https://img.shields.io/twitter/follow/CambridgeMVP.svg?style=social&label=Twitter&style=plastic)](https://twitter.com/CambridgeMVP)

Cordova plugin to show decimal keyboard on iOS devices.

Taken from [mrchandoo's](https://github.com/mrchandoo) repo [cordova-plugin-decimal-keyboard](https://github.com/mrchandoo/cordova-plugin-decimal-keyboard) and merged with [ericdesa](https://github.com/ericdesa) WKWebView fix.

Removed UIWebView code.

## Install

```bash
cordova plugin add --save cordova-plugin-decimal-keyboard-wkwebview
```

## Usage

```html
<input type="text" pattern="[0-9]*" decimal="true">
```

Input type number will not work, try to use text with [0-9] pattern instead.

<img src="screenshots/basic-usage.png" width="25%" height="25%" /> <img src="screenshots/basic-usage-typed-content.png" width="25%" height="25%" />

## Multiple decimals

```html
<input type="text" pattern="[0-9]*" decimal="true" allow-multiple-decimals="true">
```

<img src="screenshots/multiple-decimals.png" width="25%" height="25%" />

### Different decimal character

```html
<input type="text" pattern="[0-9]*" decimal="true" allow-multiple-decimals="false" decimal-char=",">
```

If you want to localize decimal character, you can change using decimal-char attribute

<img src="screenshots/different-decimal-char.png" width="25%" height="25%" />

## Known Issues
* Does not handle screen rotation.
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
