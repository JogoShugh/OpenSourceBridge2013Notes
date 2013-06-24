# Summary

[Open Source Bridge](http://opensourcebridge.org/about/) is:

> Open Source Bridge is a conference for developers working with open source technologies and for people interested in learning the open source way.
>
> Open Source Bridge is not a typical technical conference:
>
>   * It’s entirely volunteer-run, by developers, for developers.
>   * Session tracks are technology agnostic; the conference content is based around shared community experiences and similarities between projects, not differences.
>   * Proposals are public from the start, and we welcome community comments before our content team selects the featured talks.
>   * A hacker lounge is an integral part of the conference for code sprints, bug bashes, session deep dives, bouncing ideas, starting new projects or just mingling with other geeks.

# Sessions Attended

## Test Driven Development with AngularJS

Presented by Joe Eames, developer, author of [http://www.testdrivenjs.com](www.testdrivenjs.com), and author of the 
[Pluralsight AngularJS Fundamentals](http://pluralsight.com/training/Courses/TableOfContents/angularjs-fundamentals) 
course, as well as the [jQuery Advanced Topics and Testable Clientside JavaScript](http://pluralsight.com/training/Authors/Details/joe-eames) 
courses.

### Session details

Notes, links, video and slides eventually at: [http://opensourcebridge.org/sessions/1007](http://opensourcebridge.org/sessions/1007)


## Takeaways

* Talk was overflowing, most well-attended session of the day.
* Joe is working on migrating a 100,000 LOC JavaScript app, implemented with Backbone and RequireJS, into Angular, 
and states that this process is eliminating more than 50% of the code.
* AngularJS's built in support for client-side testing is impressive, and
* [Karma](http://karma-runner.github.io/0.8/index.html) is a great tool developed for this
* Works well with [Jasmine](http://pivotal.github.io/jasmine/) (designed with it in mind) -- 
similar BDD style that Mocha supports.
* Demonstrated using [Sinon.JS](http://sinonjs.org/) his tests too.

## Example test

```javascript
describe('catalogCtrl', function() {
  var ctrlConstructor, scope;

  beforeEach(module('myApp.controllers'));
  beforeEach(module('myApp.services'));

  beforeEach(inject(function($controller, $rootScope) {
    ctrlConstructor = $controller;
    scope = $rootScope.$new();
  }

it('should add the correct item to the cart with a qty of 1', fucntion () {
  var mockCart = {add: sinon.stub()};
  var mockGame = {id: 1}

  ctrlConstructor('CatalogCtrl', {$scope: scope, cart: mockCart});

  scope.add(mockGame);
  expect(mockCart.add.calledWith(1, 1)).toBe(true);
});

```

