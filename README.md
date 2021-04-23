# Matomo Vuepress Plugin for Space Elephant projects

Allows Matomo access tracking on vuepress >= 1.0. Does not work on
Vuepress 0.x, requires 1.x alpha branch with plugin support.

This project is a fork of https://github.com/qdot/vuepress-plugin-matomo, specialized for Space Elephant's projects.

## Installation

```
yarn add vuepress-plugin-matomo-spacelephant
```

## Vuepress Setup

Add the following block to the plugins array of your *config.js* file.

```js
// ...
  plugins: [
    // ... other plugins...
    [
      "vuepress-plugin-matomo-spacelephant":
      {
        'siteId': 1,
      }
    ],
    // ... more plugins...
  ]
// ...
```
## Plugin Options

* siteID (number, **Required**)
    * Matomo numeric site ID of the site you want to track
* trackerUrl (string, Optional)
    * URL where the matomo.php/matomo.js files can be found. Already configured for all Space Elephant's projects
* trackerJsFile (string, defaults to `js/`, Optional)
    * Name of the js file to call on the matomo server
* trackerPhpFile (string, defaults to `r.php`, Optional)
    * Name of the php file to call on the matomo server
* enableLinkTracking (boolean, defaults to `true`, Optional)
    * Enable/disable link click tracking
    
## License

MIT License, see [LICENSE.txt](LICENSE.txt) for more info.
