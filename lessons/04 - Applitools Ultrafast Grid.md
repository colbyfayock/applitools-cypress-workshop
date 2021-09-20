# Lesson 4 - Applitools Ultrafast Grid

We learned how we can easily add visual testing to our application with a few lines in our existing Cypress tests, which already give us testing superpowers. But not only can we test in one browser with Cypres, we can test in a wide variety of browsers all with the same test!

Crossbrowser testing is important because the different browser vendors choose to implement features ever so slightly different, meaning our website or application could look different whether it's on Chrome, Firefox, or even a mobile device.

With the Applitools Ultrafast Grid, we can make sure we're completely covered no matter what browser our visitors are using.

## Getting Started

## Objectives
* Adding additional browsers with the Ultrafast Grid
* Running tests on multiple devices in Cypress

## Exercises

### 1. Crossbrowser testing with Cypress and the Ultrafast Grid

The great thing about crossbrowser testing with the Ultrafast Grid, is we don't need to rewrite our tests multiple times. We can write our tests once and simply configure which browsers we want to use!

To do this, we'll pass an array of browsers that we want to use right into our existing `cy.open` command like:

```
browser: [
  { width: 800, height: 600, name: 'firefox' },
  { width: 1024, height: 768, name: 'chrome' },
  { deviceName: 'iPhone X' }
]
```

#### Where We'll Be Making Changes
* `demo/cypress/integration/cart.spec.js`

#### Resources
* [@applitools/eyes-cypress - Configuring the Browser](https://www.npmjs.com/package/@applitools/eyes-cypress#configuring-the-browser)
* [Applitools - Ultrafast Test Cloud](https://applitools.info/90r)

### 2. Run tests across multiple browsers

Now that we've configured out browsers, let's actually run our tests and see the results!

#### What to Run in Your Terminal
* `npm run cy:open`

_Note: remember to run your tests with your API key as we learned in Lesson 3!_
