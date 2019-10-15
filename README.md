# PPS HK Pay Bot

## Description

Pay bill via PPS HK with small amount repeatedly.

## Installation

There are 2 ways to install the extension:

### Install from Chrome Web Store

- URL: <https://chrome.google.com/webstore/detail/pps-hk-pay-bot/mlpilfangidnjfmahodhihmmaenpidgk>

### Manual Install

> Be aware that the extension will not be auto-updated if installed manually

- Download the ZIP file: <https://github.com/freehk-developer/chrome-ppshk-pay-bot/archive/master.zip>
- Unzip the ZIP file
- Go to `chrome://extensions` and turn on Developer mode at the top right corner
- Click the Load unpacked extension button and select the unzipped folder, the folder should contain `manifest.json` file
- The extension is installed

## Usage

> The extension will only work on PPS HK domain.

- Visit PPS HK website (<https://www.ppshk.com>)
- Press Login (the extension will change login buttons to visit link in current tab)
- Login to PPS HK
- Click on the extension icon next to address bar to open the popup
- Fill in the form, fill in '00' in amount input if you want to pay fixed $1
- Click Run
- Progress will be displayed in the popup

If you find login page is opened in new window, use Ctrl (Windows) / Command (Mac) + Mouse Click to open login page in new tab.

Please confirm the extension has been stopped before you close the tab / browser.
Otherwise, the extension will continue to run at the next time you visit PPS HK.

Whenever error occurs, error message will be displayed at page top, and the extension will stop running.

If you are not logged in, the extension will prepend Login links at the top of the web page,
and the extension will continue running after sign-in.

If you input incorrect / not registered bill (merchant & bill number),
PPS HK will show a failure page eventually, and the extension will stop.

## FAQ

Does the extension work on Chinese or English PPS HK website?
> It works on both languages website.

What if my bill is not on the first page of the bill table?
> It will still work as the choose bill process is using form submit instead of simulating button press.

Can I leave the tab in background?
> Better keep the tab active. It is okay for a short period of time, but for a longer time, Chrome may do performance throttling on background tabs, which would lead to unknown behaviour.

## Remark

As there is no difference in form data when choosing different instalment,
no input field will be provided for that.

The extension may no longer work if PPS HK updates the website.
