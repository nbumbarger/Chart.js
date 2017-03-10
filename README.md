# Chart.js with Error Bars

*This is an fork of [Chart.js](http://www.chartjs.org) which supports error bars. It can be used as a stand-alone library or as an extension of the original library.

The master branch is compatible with Chart.js 2.x.x. There are branch compatible with earlier versions, but I will not maintain them.

# Chart.js

[![Build Status](https://travis-ci.org/chartjs/Chart.js.svg?branch=master)](https://travis-ci.org/chartjs/Chart.js) [![Code Climate](https://codeclimate.com/github/nnnick/Chart.js/badges/gpa.svg)](https://codeclimate.com/github/nnnick/Chart.js) [![Coverage Status](https://coveralls.io/repos/github/chartjs/Chart.js/badge.svg?branch=master)](https://coveralls.io/github/chartjs/Chart.js?branch=master)

[![Chart.js on Slack](https://img.shields.io/badge/slack-Chart.js-blue.svg)](https://chart-js-automation.herokuapp.com/)
>>>>>>> 1ca0ffb5d5b6c2072176fd36fa85a58c483aa434

## Documentation

You can find documentation for Chart.js at [nnnick.github.io/Chart.js/docs-v2/](http://nnnick.github.io/Chart.js/docs-v2/). Usage of the extension is noted below.

## Include Error Bars

Including error bars is extremely simple. Download *this* version of Chart.js and include it in your site. To add error bars, include an array called `error` (of the same length as the `data` array) in each dataset.
=======
You can download the latest version of Chart.js from the [GitHub releases](https://github.com/chartjs/Chart.js/releases/latest) or use a [Chart.js CDN](https://cdnjs.com/libraries/Chart.js).

To install via npm:

```bash
npm install chart.js --save
```

To install via bower:
```bash
bower install chart.js --save
```

#### Selecting the Correct Build

Chart.js provides two different builds that are available for your use. The `Chart.js` and `Chart.min.js` files include Chart.js and the accompanying color parsing library. If this version is used and you require the use of the time axis, [Moment.js](http://momentjs.com/) will need to be included before Chart.js.

The `Chart.bundle.js` and `Chart.bundle.min.js` builds include Moment.js in a single file. This version should be used if you require time axes and want a single file to include, select this version. Do not use this build if your application already includes Moment.js. If you do, Moment.js will be included twice, increasing the page load time and potentially introducing version issues.

Options included with this version of the library:

    //String - direction of the error bars. "up", "down", or "both"
    errorDir : "both",

You can find documentation at [www.chartjs.org/docs](http://www.chartjs.org/docs). The markdown files that build the site are available under `/docs`. Previous version documentation is available at [www.chartjs.org/docs/#notes-previous-versions](http://www.chartjs.org/docs/#notes-previous-versions).

    //Number - stroke width of the error bars
    errorStrokeWidth : 1,

    //String - color of the error bar in hex or RGBA.
    //If not specified defaults to the fill color of the bar of point.
    errorColor: "rgba(220, 220, 220, 1)"

Before submitting an issue or a pull request to the project, please take a moment to look over the [contributing guidelines](https://github.com/chartjs/Chart.js/blob/master/CONTRIBUTING.md) first.

    //Number - ratio of the width of the error bar caps to the width of the bar
    errorCapWidth : 0.75,
    //For line charts, errorCapWidth is the ratio of the width of the error bar
    //caps to the radius of the points, and the default is 2.5.

## Compatibility

This repo is compatible with @nnnick/Chart.js **v2.0**, so even if you are already using Chart.js on your site, switching to my version will not harm anything.

## Building and Testing

To build, run `gulp build`.

To test, run `gulp test`.

To test against code standards, run `gulp lint`.

More information on building and testing can be found in [gulpfile.js](gulpfile.js).

Thanks to [BrowserStack](https://browserstack.com) for allowing our team to test on thousands of browsers.

## License

Chart.js, and this exension, are available under the [MIT license](http://opensource.org/licenses/MIT).

## Bugs & issues

When reporting bugs or issues, if you could include a link to a simple [jsbin](http://jsbin.com) or similar demonstrating the issue, that'd be really helpful.
