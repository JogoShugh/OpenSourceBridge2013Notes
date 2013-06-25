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

# Memorable Sessions Attended

There were lots of sessions at the conference. Some sessions that I attended were more memorable than others. These 
are my notes from those.

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

## Expanding Your Empathy

Presented by [Kronda Adair](http://karveldigital.com/), web developer, Portland native. 
Blogs at [http://kronda.com/](kronda.com/). 

### Session details

Session: [http://opensourcebridge.org/sessions/1148](http://opensourcebridge.org/sessions/1148)
Slides: [https://speakerdeck.com/kronda/expanding-your-empathy](https://speakerdeck.com/kronda/expanding-your-empathy)

### Description

> "I believe empathy is the core competency that is missing from much of the efforts to push the tech community in a direction towards more diversity of all kinds. Companies, communities and conferences cannot expect everything to magically change until they’re willing to go deep and examine the systemic patterns and structures that keep underrepresented communities from feeling safe and welcome in the tech space."

### Takeaways

I was not sure what to expect from this talk. I thought it would be about expanding empathy for end-users, though it 
seemed to be more about empathy for fellow open-source citizens.

* Discussed her experience as "Portland's only black, lesbian software developer" -- Portland has a less than 6%
African American population
* Exercise on "microaggressions" -- someone poking the arm of another who was trying to correct spelling errors in
a document. -- made the task take much, much longer than someone not being poked
 * Analog to daily self-question of: "Do I spend my time trying to combat these microaggressions, or do I just try 
 do what I really want to do -- develop software to the best of my ability?"
* When you offend someone: stop, listen, apologize
* Don't "mansplain" things to women in tech (or in general)
* Don't be the "tone police" -- "Why can't you stop being so angry?" or "I could understand if you stopped being so angry."
* Don't "derail" -- belittling ambitions of someone who doesn't fit your stereotypical tech worker ideas
* Example: Kronda went to a Drupal conference and was walking toward the door when the man working the door looked 
puzzled and asked "Are you here with your husband?" before letting her enter.
* She told story of how she used the phrase "Low man on the totem pole" as a Native Amercian friend of hers 
interviewed her. Oops. (And, a cursory look at the history of totem poles shows that lower-down depections are often **more**
important than ones higher up on the pole.)

### Links

* [http://geekfeminism.wikia.com/wiki/Geek_Feminism_Wiki](Geek Feminism Wiki)
* [http://www.understandracism.org/](Uniting to Understand Racism)
* [http://revisionpath.com/](Revision Path -- a weekly showcase of the world's black graphic designers, web designers, and web developers (Atlanta based)

## Innovating Faster with a Micro-Service Architecture using SBT, Continuous Delivery, and LXC

## Training the Trainers

## How My Kids are Learning to Program by Talking

## Designgenineering

## Unconference: Open source for underserved communities

## Unconference: Hadoop and Big Data processing

## Unconference: AngularJS and fighting disease
