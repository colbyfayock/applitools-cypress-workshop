# Lesson 2: Testing with Cypress

[Cypress](https://www.cypress.io/) is a powerful testing framework that allows us to run tests right inside of a browser.

We can use it to make sure we're covering not only how the code renders, but how the code runs!

## Getting Started

## Objectives
* Review and run existing Cypress tests
* Add and review a visual bug

## Exercises

### 1. Review and run existing Cypress tests

Running our tests right inside a real browser is important, as we don't want to just simulate what our application _could_ do, but how it's actually working.

In this repository, we already have a Cypress test set up pointed to a demo application. Let's see how this works by running our existing tests!

#### Where To Look
* `demo/cypress/integration/cart.spec.js`

#### What to Run in Your Terminal
* `npm run cy:open`

_Note: make sure you navigate to the top of the `demo` directory before trying to run this command!_

#### Resources
* [cypress.io](https://www.cypress.io/)
* [Workshop Demo](https://applitools-cypress-workshop-demo.netlify.app/)


### 2. Introduce a visual bug into the demo application and re-run tests

Web development and browsers are complicated in how they work. What happens if the rendered code works but the UI still looks broken?

As great as Cypress is (and it's pretty great), it's not able to actually SEE what is inside of the browser.

We'll introduce a change to the demo application and re-run our tests to see how this can impact our tests.

#### What to Run in Your Terminal
* `npm run cy:open`

_Note: make sure you navigate to the top of the `demo` directory before trying to run this command!_

#### Where To Make a Change
* `demo/cypress/integration/cart.spec.js`

Update the URL on line 5 to:
```
https://deploy-preview-1--applitools-cypress-workshop-demo.netlify.app/
```

> Want to see the change that was made? Check out the Pull Request for the visual bug at: https://github.com/colbyfayock/applitools-cypress-workshop-demo/pull/1
