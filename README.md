# \<pf-event-cal\>



## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.
## Example
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="pf-event-cal.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
 <pf-event-cal
                  data='[
                          { "eventName": "Lunch Meeting w/ Mark", "calendar": "Work", "color": "orange","date":"1491322091394" },
                          { "eventName": "WI vs Pak", "calendar": "sport", "color": "blue","date":"1499185140000" },
                          { "eventName": "WI vs Pak", "calendar": "sport", "color": "blue","date":"1491581940000" },
                          { "eventName": "Public Holiday", "calendar": "holiday", "color": "green","date":"1494173940000" }]'
          >

          </pf-event-cal>
```
### Styling
The following custom properties and mixins are available for styling:

Custom property                         | Description                             | Default
----------------------------------------|-----------------------------------------|-------------------------
`--pf-calendar-bg-color`                |  Calendar background                    | #4A4A4A
`--pf-calendar-width`                   |  Calendar Width                         | 420px
`--pf-calendar-height`                  |  Calendar Height                        | 570px
`--pf-calendar-header-background`       |  Calendar Header Background             | rgba(66, 66, 66, 1)
`--pf-calendar-header-left-arrow-color` |  Previous Month arrow color             | rgba(160, 159, 160, 1)
`--pf-calendar-header-right-arrow-color`|  Next Month arrow color                 | rgba(160, 159, 160, 1)
`--pf-calendar-month-title-color`       |  Month Title color                      | #000
`--pf-calendar-week-bg`                 |  Background color of week               | #4A4A4A
`--pf-calendar-day-bg`                  |  Day Background                         | #4A4A4A
`--pf-calendar-other-day-color`         |  color of previous and next month date  | rgba(255, 255, 255, .3)
`--pf-calendar-day-color`               |  color of date                          | #000
`--pf-calendar-today-color              |  Current date Color                     | rgba(156` 202, 235, 1)
`--pf-calendar-day-name-color           |  Name of Day color e.g(MON,TUE,WED)     | rgba(255` 255, 255, .5)
`--pf-calendar-event-detail-bg`         |  Event box background                   | rgba(164, 164, 164, 1)
`--pf-calendar-no-event-color`          |  color of label "NO Event"              | #000
`--pf-calendar-legend-bg`               |  Background color of legend bar         | rgba(60, 60, 60, 1)

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
