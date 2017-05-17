
# pf-elements
A Polymer 2.0 based collection of reusable web components 

[![Join the chat at https://gitter.im/pf-elements/Lobby](https://badges.gitter.im/pf-elements/Lobby.svg)](https://gitter.im/pf-elements/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/PFElements/pf-calendar-events)
[![Polymer Version](https://img.shields.io/badge/polymer-v2-blue.svg)](https://www.polymer-project.org)

## Demo
[Click here for Demo](https://www.webcomponents.org/element/PFElements/pf-calendar-events/demo/demo/index.html)


## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

# PF Calendar Events

An Advanced/composite Polymer 2.0 based custom elements that can be used to set Events/appointments/meetings in a calendar. 

| Element Name | Latest Version (Bower) | Npm version  | Build Status |
|--------------|------------------------|--------------|--------------|
| [pf-calendar-events](https://github.com/PFElements/pf-calendar-events) | [![GitHub version](https://badge.fury.io/gh/PFElements%2Fpf-calendar-events.svg)](https://badge.fury.io/gh/PFElements%2Fpf-calendar-events) | [![npm version](https://badge.fury.io/js/pf-calendar-events.svg)](https://www.npmjs.com/package/pf-calendar-events) |[![Build Status](https://travis-ci.org/PFElements/pf-calendar-events.svg?branch=master)](https://travis-ci.org/PFElements/pf-calendar-events) | 

## Learn more

See the list of elements, demos, and documentation by browsing this collection on webcomponents.org:

### [Take me to webcomponents.org ›](https://www.webcomponents.org/element/PFElements/pf-calendar-events)

---
# Customization and usage

`<pf-calendar-events></pf-calendar-events>` can be customized in a number of ways

## Customization of look and feel

By default you have two general options

a. material-calendar

b. classic-calendar

Once you decide you general look and feel then you can further customize the details, e.g. if you chose a Material Design look and feel and you want to change the width, hight, color etc. you can do that with the provided API. 
#### Material Calendar Example
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="pf-calendar-events.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html




 <pf-calendar-events
                  calendarstyle="material-calendar"
data='[
                          { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1491322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1491322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1491322091394" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1492196400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1492455600000" },
                          { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1495322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1495322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1495047600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1495196400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1495455600000" },
                           { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1497322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1497322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1497047600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1497196400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1497455600000" },
                           { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1500322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1500322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"150047600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"150096400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"15005600000" },
                            { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1502922091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1502922091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1502947600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1502996400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1502955600000" },
                          { "eventName": "Appoint ment With Dr David", "category": "Medical", "color": "yellow","date":"1499185140000" },
                          { "eventName": "Soccer Match", "category": "holiday", "color": "green","date":"1492887600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1494173940000" }]'
          >

          </pf-calendar-events>
```
#### Classic Calendar Example
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="pf-calendar-events.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
 <pf-calendar-events
                  calendarstyle="classic-calendar"
                  data='[
                          { "eventName": "Lunch Meeting w/ Mark", "calendar": "Work", "color": "orange","date":"1491322091394" },
                          { "eventName": "Giants vs Packers", "calendar": "sport", "color": "blue","date":"1499185140000" },
                          { "eventName": "Soccer", "calendar": "sport", "color": "blue","date":"1491581940000" },
                          { "eventName": "Public Holiday", "calendar": "holiday", "color": "green","date":"1494173940000" }]'
          >

          </pf-calendar-events>
```
default value of 'calendarstyle' is 'material-calendar'
### Types of calendar
You can define different types of calendar events (appointments, meetings, reminders, etc). e.g. you can define a "Sports" Calendar "Office Meeting" calendar, "Birthday Reminders" calendar. Distinct type of categories will appear in different colors.

### CRUD operations

Buttons / icons are provided to enable Adding, deleting or updating an event (meeting, reminder, appointment etc)
Material based button and icons are provided to enable these operations.
For firebase events data, please see our firebase element

## Customization of Calendar Events/Data (your meetings, appointments, reminders etc)

Of course if you cannot provide you own data then why even use a third party component, and you need events as well to notify you of the user interaction with the calendar

This custom element provides you two generic ways that again can be further customized

a. Data Through firebase custom element (Please see our firebase custom element that can be combined with this element to enable your data interaction from firebase

b. By providing an array of data. (Calendar events, appointments, meetings, reminders etc.)

### CRUD operations
Our custom element provides a way to hook your CRUD operations into our calendar, it provides a number of API hooks/events to notify you about an operation that is performed on a certain event.


Custom Event                     | Description                       
---------------------------------|----------------------------------------
`event-add`                      | Add event retuns current selected date ('e.detail.date'), fired when user press add event button  
`event-edit`                     | Edit event retuns event ('e.detail.event'),fired when user press edit event button
`event-delete`                   | Delete event retuns event ('e.detail.event'),fired when user press delete event button
`event-select`                   | Event Select retuns event ('e.detail.event'),fired when user click on any event            
`date-select`                    | Date Select retuns seleted date and events of date ('e.detail.date'and'e.detail.events'),fired when user click on any event             
  


<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="pf-calendar-events.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html




 <pf-calendar-events
data='[
                          { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1491322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1491322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1491322091394" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1492196400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1492455600000" },
                          { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1495322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1495322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1495047600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1495196400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1495455600000" },
                           { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1497322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1497322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1497047600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1497196400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1497455600000" },
                           { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1500322091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1500322091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"150047600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"150096400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"15005600000" },
                            { "eventName": "Lunch Meeting W/ Mark", "category": "Work", "color": "orange","date":"1502922091394" },
                          { "eventName": "Rob Birthday  ", "category": "Birthday", "color": "blue","date":"1502922091394" },
                          { "eventName": "Appointment With Dr David", "category": "Medical", "color": "yellow","date":"1502947600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1502996400000" },
                          { "eventName": "Due date of Project Dilivery", "category": "Work", "color": "orange","date":"1502955600000" },
                          { "eventName": "Appoint ment With Dr David", "category": "Medical", "color": "yellow","date":"1499185140000" },
                          { "eventName": "Soccer Match", "category": "holiday", "color": "green","date":"1492887600000" },
                          { "eventName": "Public Holiday", "category": "holiday", "color": "green","date":"1494173940000" }]'
          >

          </pf-calendar-events>
```
Custom property                         | Description                             | Default
----------------------------------------|-----------------------------------------|-------------------------
`--pf-calendar-bg-color`                |  Calendar background                    | #4A4A4A
`--pf-calendar-width`                   |  Calendar Width                         | 420px
`--pf-calendar-height`                  |  Calendar Height                        | 570px
`--pf-calendar-header-background`       |  Calendar Header Background             | rgba(66, 66, 66, 1)
`--pf-calendar-header-height`           |  Calendar Header height                 | 50px
`--pf-calendar-month-title-font-size`   |   Font size of  month on header         | 20px
`--pf-calendar-month-title-line-height` |  Calendar Header title line Height      | rgba(66, 66, 66, 1)
`--pf-calendar-header-left-arrow-color` |  Previous Month arrow color             | rgba(160, 159, 160, 1)
`--pf-calendar-header-right-arrow-color`|  Next Month arrow color                 | rgba(160, 159, 160, 1)
`--pf-calendar-month-title-color`       |  Month Title color                      | #000
`--pf-calendar-week-bg`                 |  Background color of week               | #4A4A4A
`--pf-calendar-day-bg`                  |  Day Background                         | #4A4A4A
`--pf-calendar-day-color`               |  color of date                          | #000
`--pf-calendar-other-day-color`         |  color of previous and next month date  | rgba(255, 255, 255, .3)
`--pf-calendar-today-color`             |  Current date Color                     | rgba(156` 202, 235, 1)
`--pf-calendar-day-name-color`          |  Name of Day color e.g(MON,TUE,WED)     | rgba(255` 255, 255, .5)
`--pf-calendar-event-detail-bg`         |  Event box background                   | rgba(164, 164, 164, 1)
`--pf-calendar-event-color`              |  color of label "Event"                | #000
`--pf-calendar-addevent-button-bg-color'|  Add Event Button color                 | rgba(164, 164, 164, 1)
`--pf-calendar-addevent-button-text-color`| Add Event text color                  | #fff
`--pf-calendar-addevent-button-hover-color`|  Add event button hover color        | rgba(170, 170, 170, 1)
`--pf-calendar-addbutton-disply`        |  to hide button set "none"              |inline-block
`--pf-calendar-deletebutton-disply`     |  to hide button set "none"              |inline
`--pf-calendar-editbutton-disply`       |  to hide button set "none"              |inline
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

## Contributing

Comments, questions, suggestions, issues, and pull requests are all welcome.

* Give us a **Star on GitHub**.



### Get in touch with the team

Joing us at [![Join the chat at https://gitter.im/pf-elements/Lobby](https://badges.gitter.im/pf-elements/Lobby.svg)](https://gitter.im/pf-elements/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

- [Twitter](<a href="https://twitter.com/polymerio" class="twitter-follow-button" data-show-count="false">Follow @polymerio</a>)
- [Facebook] (https://www.facebook.com/polymerjs)
- [Google+] (https://plus.google.com/116168214823506639166) 
- [YouTube] (https://www.youtube.com/channel/UCDKqvDyAn_QTBvCPvrZKTkw) 
- [Website] (https://polymerjs.io)

### Some ways to help:

- **Test the elements and provide feedback**: We would love to hear your feedback on anything related to the elements, like features, API and design. The best way to start is by trying them out. And to get a quick response, either drop a question/comment on the chat or open an issue in GitHub.
- **Report bugs**: File issues for the elements in their respective GitHub projects.
- **Send pull requests**: If you want to contribute code, check out the development instructions below.

We encourage you to read the [contribution instructions by GitHub](https://guides.github.com/activities/contributing-to-open-source/#contributing) also.

## License

MIT License
