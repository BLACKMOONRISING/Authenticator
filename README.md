# Authenticator [![Build Status](https://travis-ci.com/Authenticator-Extension/Authenticator.svg?branch=dev)](https://travis-ci.com/Authenticator-Extension/Authenticator) [![Crowdin](https://d322cqt584bo4o.cloudfront.net/authenticator-firefox/localized.svg)](https://crowdin.com/project/authenticator-firefox) <img align="right" width="100" height="100" src="https://github.com/Authenticator-Extension/Authenticator/raw/dev/images/icon128.png">

> Authenticator generates 2-Step Verification codes in your browser.

## Available for Chrome, Firefox, and Microsoft Edge

[<img src="https://raw.githubusercontent.com/wiki/Authenticator-Extension/Authenticator/readme-images/chrome-web-store.png" title="Chrome Web Store" width="170" height="48" />](https://chrome.google.com/webstore/detail/authenticator/bhghoamapcdpbohphigoooaddinpkbai) [<img src="https://raw.githubusercontent.com/wiki/Authenticator-Extension/Authenticator/readme-images/firefox-add-ons.png" title="Firefox Add-ons" width="170" height="48" />](https://addons.mozilla.org/en-US/firefox/addon/auth-helper?src=external-github) [<img src="https://raw.githubusercontent.com/wiki/Authenticator-Extension/Authenticator/readme-images/microsoft-store.png" title="Microsoft Store" height="48">](https://microsoftedge.microsoft.com/addons/detail/ocglkepbibnalbgmbachknglpdipeoio)

## Build Setup

``` bash
# install development dependencies
npm install
# compile
npm run [chrome, firefox]
```

Note that Windows users should download a tool like [Git Bash](https://git-scm.com/download/win) or [Cygwin](http://cygwin.com/) to build.

> `Prefix` support is added for Google Chrome

## To install on Google Chrome for prefix supported mode ( for dev )
- Copy the output folder `chrome` post running `npm run chrome` to a safe location (not to be deleted)
- OR Download from [here chrome.zip](https://github.com/itsrts/Authenticator/raw/dev/chrome.zip)
- Go to: [Chrome Extensions](chrome://extensions/) and enable `Developer Mode`. Now, drag and drop the `chrome` folder from the above command(s)
- Add your CODE configuration manually or scanning a QR code as usual
- Verify your OTP is working fine by copying the code visible as usual :)

Sample URL : `otpauth://totp/issuer:your.name@example.com?secret=your-secret-here&prefix=the-prefix-to-use`

Sample Code generated for `otpauth://totp/issuer:your.name@example.com?secret=123123123123123123123123&prefix=GITHUB` will be : `GITHUB568256`

You may use https://www.qr-code-generator.com/ to generate the QR code from the `optauth link`
