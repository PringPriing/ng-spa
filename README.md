ng-spa 0.5
==========

Single page application (SPA) demo built with ASP.NET Web API 2 and AngularJS.

Technologies
============

API
---

* ASP.NET Web API 2
* EF 6 Code First 
* AutoMapper
* Autofac

SPA App
--------

* AngularJS
* Semantic UI
* Gulp.js
* Jasmine

Building the application
============

API
---

1. Build the solution to install Nuget packages.(This will automatically restore Nuget packages. Please ensure you have    Nuget version 2.7 or higher)
2. The Project ResourceMetada.API is configured to run using IIS Express.
3. Before starting the Client Application (ResourceMetadata.Web), please ensure that the API project is running in IIS     or IIS express.

SPA App
-------
      
1. Config.js file at  ***[source/ResourceMetadata/ResourceMetadata.Web/Scripts/config.js](https://github.com/shijuvar/ng-spa/tree/master/source/ResourceMetadata/ResourceMetadata.Web/Scripts/config.js)*** holds the api url used by the Client application. Update this file to change the api url appropriately.
2. If you haven't installed Node.js, download and install it from http://nodejs.org/
3. Navigate to the directory of ResourceMetadata.Web project ***[source/ResourceMetadata/ResourceMetadata.Web/](https://github.com/shijuvar/ng-spa/tree/master/source/ResourceMetadata/ResourceMetadata.Web/)*** in command prompt.
4. Run command **npm install**
5. Execute gulp tasks
    1. Run command **gulp build**.
    2. In order to clean the destination files created by build task, run **gulp cleanbuild**.
    3. To run unit tests, run the command **gulp tests** 
