Wikimetrics Chart
=================
wikimetrics-chart is a web component that graphs data about Wikipedia's editor activity. 

The component uses google charts API to graph. 

The data graphed is served by [Wikimetrics](https://metrics.wmflabs.org/).

To use:

* Install bower
    ```
    npm install -g bower
    ```

* Install wikimetrics component 
    ```
    bower install wikimetrics-chart
    ```

This will install wikimetrics-chart and all its dependencies to ./bower-components

* Use wikimetrics-chart in your page. An example of usage:
    
```
    <head> 
        <title> Google Chart visualization of Newly Registered Users via Web Component</title>
        <script src="./bower_components/platform/platform.js"></script>
        <link rel="import" href="./bower_components/wikimetrics-chart/wikimetrics-chart.html">
         
    </head>
    <body unresolved>
         <wikimetrics-chart
           type='line'
           height='300px'
           width='400px'
           metric ='["NewlyRegistered"]'
           data = '["rowiki","ruwiki"]'
         </wikimetrics-chart> 
    </body>

    </html>
```

Info
-----
Prototype displays [Newly Registered User](https://meta.wikimedia.org/wiki/Research:Newly_registered_user)
data.

Datafiles are included with prototype at this time. Data will be feched from wikimetrics once public
data is available on the production instance.

Public files are deployed (for now)
only to [Wikimetrics Staging] (https://metrics-staging.wmflabs.org/static/public/datafiles/)


