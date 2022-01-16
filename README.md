# Chrome Extension Angular

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.1.3.

## Quick Start

- Quick Start
  - Clone this repo
  - Install packages `npm install`
  - Build `npm run build`
  - Load extension in Chrome

### Notes

- Notes
  - Create from scratch
    - Create an angular app `npx -p @angular/cli ng new angular-extension --style=scss`
    - Create a `manifest.json` file with similar contents in the `/src` folder
    - Add `src/manifest.json` to `angular.json` `project/.../architect/build/options/assets`
    - Build `npm run build` or watch `npm run watch`
    - Load extension in Chrome
      - Open Chrome
      - Open the Extensions Management page by navigating to `chrome://extensions`
      - Enable Developer Mode by toggling the switch next to Developer Mode
      - Click the Load unpacked button and select the extension directory (dist/angular-chrome-extension)
      - You should be able to see the extension in Chrome
    - If you change the `manifest` you have to reload the extension, if you change any source file open and close the popup
  - Deploy
    - Need a better way than copying the dist folder and loading the extension in raw format
    - Also the production deployment is not loading the material design icons

#### References

- References
  - Google Chrome Extensions API Reference
    - [chrome.cookies](https://developer.chrome.com/docs/extensions/reference/cookies/)
  - [Chrome Extensions samples](https://github.com/GoogleChrome/chrome-extensions-samples)
  - [Chrome Extension with Angular — from Zero to a Little Hero](https://www.justjeb.com/post/chrome-extension-with-angular-from-zero-to-a-little-hero)
    - [GitHub source code](https://github.com/just-jeb/angular-chrome-extension)
