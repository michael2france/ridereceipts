<p align="center"><img src="/uber-run.png" alt="Uber Run" width="150"></p>

<p align="center">
<a href="https://travis-ci.org/break-enter/uberrun">
<img src="https://travis-ci.org/break-enter/uberrun.svg?branch=master">
</a>
<a href="https://codeclimate.com/github/break-enter/uberrun/maintainability">
<img src="https://api.codeclimate.com/v1/badges/a176f7fdd72bd288291f/maintainability" />
</a>
<a href="https://david-dm.org/break-enter/uberrun">
<img src="https://david-dm.org/break-enter/uberrun.svg" />
</a>
<a href="https://david-dm.org/break-enter/uberrun?type=dev" title="devDependencies status"><img src="https://david-dm.org/break-enter/uberrun/dev-status.svg"/></a>
</p>


> Simple automation desktop app to download and organize your tax invoices from Uber.


![screenshot](/uberrun.gif)

### Download

MacOS - [https://github.com/break-enter/uberrun/releases](https://github.com/break-enter/uberrun/releases)

Chromium - See Requirement below

Linux and Windows build coming soon

## Why

For businesses and sole proprietors it is sometimes pain to download invoices for their taxes from Uber with their current user interface. They have to manually go each trip and download it.

## Solution

Automation. We made this desktop app to automate the task of downloading invoices and save it one place versus manually going to Uber account and scan through each and every trips in order to download invoice.

## Requirements

Since Electron is not 100% headless. We are using [Google Puppeteer](https://github.com/GoogleChrome/puppeteer) to scrape website.

In order to make app work please download [Chromium](https://download-chromium.appspot.com/) and extract folder on your desktop.

## Limitation

Currently program would grab invoices whatever is available on Uber's site. Invoices that are "*expired*", *cancelled*, Uber Eats or has "*Request invoice*" option would be skipped from downloading.

You might also be halted by Uber's rate limiting. So please try to use this application in certain amount of gap.

## Note

This app doesn't store any credentials anywhere. This application is fully without database and it is solely automating on chromium browser as you type.

## Features

- [x] Categorized by User Account
- [x] Categorized by Year and Month
- [x] Invoice File name by Month, Date and Timestamp
- [x] Filter by specific Month available on Uber
- [ ] Including Uber eats invoice
- [ ] Configurable Path to Save Invoices

## Developer Notes

#### Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:9080
npm run dev

# build electron application for production
npm run build


# lint all JS/Vue component files in `src/`
npm run lint

```

## Credits

- Adi Ofir ([@breakenterTo](https://twitter.com/breakenterTo)) for logo and all design related contributions.

## Support / Contribution

Please feel free to give suggestion or report bug by [creating issue](https://github.com/break-enter/uberrun/issues) or letting me know on twitter [@mrgodhani](https://twitter.com/mrgodhani).

## License
[MIT](https://github.com/break-enter/uberrun/blob/master/LICENSE)
