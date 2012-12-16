#The ideal single page JavaScript application

A collection of notes and links on the topic of building a maintainable single page application with JavaScript.

## Style frameworks 

http://compass-style.org/

http://foundation.zurb.com/
https://github.com/csswizardry/inuit.css/

http://bradfrost.github.com/this-is-responsive/resources.html

http://www.metaltoad.com/blog/simple-device-diagram-responsive-design-planning

http://www.getskeleton.com/

http://webdesign.tutsplus.com/articles/design-theory/designing-for-a-responsive-web/

http://designshack.net/articles/css/which-is-right-for-me-22-responsive-css-frameworks-and-boilerplates-explained/

http://thesassway.com/advanced/building-a-css-framework-with-sass

https://gist.github.com/1309546


## Modularization 

http://www.slideshare.net/nzakas/scalable-javascript-application-architecture

JavaScript +  HTML + CSS

* Any single module should be able to live on its own, ex. Weather module, stock module
* Each module should not affect another module directly
* Each module should run its own sandbox
* Loose coupling between modules
* Each part of the architecture is like a puzzle piece. No single piece needs to know what the picture is. All that matters is that the piece does its own job correctly.
* The web application is created as result of all parts doing their job.

## SEO 

http://backbonetutorials.com/seo-for-single-page-apps/

## Frameworks evaluation criteria 

How many standard components will be used?
Can those components be easily implemented or replaced with third-party components.

Does it support two-way binding?

Does it support composite views/components?

Does it support model-driven view?

View must be unit testable without appending to the DOM tree.
* Modularization
* Loose coupling

http://angular-ui.github.com/

## Architecture

http://developer.chrome.com/apps/app_frameworks.html

http://code.google.com/p/mdv/

http://addyosmani.com/blog/digesting-javascript-mvc-pattern-abuse-or-evolution/

http://www.alexatnet.com/articles/model-view-controller-mvc-javascript

http://addyosmani.com/resources/essentialjsdesignpatterns/book/

https://github.com/addyosmani/essential-js-design-patterns

http://addyosmani.com/largescalejavascript/

http://singlepageappbook.com/

http://www.slideshare.net/mahemoff/webfirst-design-patterns

http://softwareas.com/automagic-event-registration

Configurable views and features in views – support responsive design

State machine?

Model-driven view approach – views care only the model, and views should communicate through model changes.

Local data store – provide CRUD operations for client side code, and synchronize the data from the server.

## Performance 

Use CDN, cache resource locally

Use phantomJs, zombie, or jsdom to generate certain views and cache on the server. Return the cached views as HTML and CSS to client for fast loading experience, then bootstrap the needed scripts and resources for any subsequent UI.

## Testing 

Jasmine tests to run the UI with mock data. Run the tests in JsTestDriver for browser compatibility

Webdriver tests with ghostdriver for fast happy path tests

Use setTimeout to control the delay time of Ajax calls to mimic network latency, which allow usability testing under slow network

## Misc 

https://github.com/addyosmani/aura

https://github.com/tbranyen/backbone.layoutmanager

Cache deferred

Lime.js  Meteor.js

## Gathering Requirement and Creating Mockups 

If existing UI exist, look at the workflow and UI, see 
* What are essential?
* What improvements are needed?
* What can be removed?

Look at UI design patterns for ideas

## Dependency Injection

http://docs.angularjs.org/guide/di

http://blog.jankuca.com/post/23066002249/dependency-injection-javascript

http://modernjavascript.blogspot.com/2012/10/dependency-injection-in-closure-ioc.html

https://github.com/rhysbrettbowen/Loader

http://maxpolun.com/js/2012/10/17/a_javascript_dependency_injection_framework_in_under_20_lines_of_code.html

http://merrickchristensen.com/articles/javascript-dependency-injection.html

http://deftjs.org/

https://github.com/cujojs/wire

## Promising Frameworks

[Ember.js](http://emberjs.com)

[Knockback.js](http://kmalakoff.github.com/knockback)

[Angular.js](http://angularjs.org/)

## Other Frameworks

https://github.com/cujojs/curl

http://www.ubelly.com/2011/11/scalablejs/

http://en.wikipedia.org/wiki/Single-page_application

http://www.youtube.com/watch?v=vXjVFPosQHw

http://boilerplatejs.org/

http://scaleapp.org/

http://www.slideshare.net/rohitsghatol/building-single-page-applications

http://programmers.stackexchange.com/questions/144717/advantages-and-disadvantages-of-building-a-single-page-web-application

http://css-tricks.com/one-page-apps-i-actually-use/

http://www.dzone.com/mz/dotnet

http://qconsf.com/

http://velocityconf.com/

http://www.ibm.com/developerworks/rational/library/3100.html

http://www.html5rocks.com/en/
