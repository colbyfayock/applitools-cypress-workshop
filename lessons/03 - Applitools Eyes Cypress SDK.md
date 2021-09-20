# Lesson 3 - Applitools Eyes Cypress SDK

The good news, is it's not too much of a lift to add visual tests, in fact, we can add those visual tests right to our existing tests!

While Applitools supports a [wide variety of SDKs](https://applitools.com/tutorials), we'll be looking at how we can add visual tests with the [Eyes Cypress SDK](https://www.npmjs.com/package/@applitools/eyes-cypress).

## Getting Started

## Objectives
* Install the SDK
* Add a visual test
* Run our first test
* View test results

## Exercises

### 1. Installing the Applitools Eyes Cypress SDK

Installing the Eyes Cypress SDK is as easy as running 2 commands!

We'll see how we acn easily configure our project so we can dive right into adding our first Eyes check.

#### What to Run in Your Terminal
* `npm install -D @applitools/eyes-cypress`
* `npx eyes-setup`

#### Resources
* [@applitools/eyes-cypress](https://www.npmjs.com/package/@applitools/eyes-cypress)

### 2. Adding our first visual test with Eyes

The best part about the Applitools Cypress integration is Eyes is available as Cypress commands, just like how you would run anything else in Cypress!

If you try to imagine a camera lens (or an eye 👁), we want to first open up our lens, take our picture, and finally close our lens.

The same concept applies to Applitools Eyes, where we'll want to first open our Eyes, check our page, then close our Eyes right back up.

#### Where We'll Be Making Changes
* `demo/cypress/integration/cart.spec.js`

#### Resources
* [@applitools/eyes-cypress Usage](https://www.npmjs.com/package/@applitools/eyes-cypress#usage)

### 3. Running Cypress tests with Applitools

Running our visual tests with Cypress is just about exactly the same as we normally would run tests except one small difference, we need to set our Applitools API key!

To do this, we'll first need an Applitools account, where we'll then find our API key, and then use that API key to run our Cypress tests.

While running our tests, we'll see how our visual tests work with the visual bug in our demo and without, to see how we can see our results.

#### What to Run in Your Terminal

Before running your test, you need to make your API key available to the environment. You can do this by either prepending your test command or exporting it in your terminal session.

To prepend, run the command like:

```
APPLITOOLS_API_KEY="[Your Key]" npm run cy:open
```

To export your API key on a Mac, run:

```
export APPLITOOLS_API_KEY="[Your Key]"
```

To export your API key on Windows, run:

```
set APPLITOOLS_API_KEY="[Your Key]"
```

If exporting, you can then run your test command normally as:
```
npm run cy:open
```

#### Resources
* [Applitools - Create a Free Account](https://auth.applitools.com/users/register)
* [Applitools - Setting Up Your Environment](https://applitools.com/tutorials/getting-started/setting-up-your-environment.html)

> Psst: need the URL for the visual bug again?
```
https://deploy-preview-1--applitools-cypress-workshop-demo.netlify.app/
```

### 4. Viewing new test results in the Applitools Dashboard

Now that we ran our first set of tests, we want to ultimately see what the results look like inside of our dashboard!

Applitools is rich with features to help you not only see visual differences, but also debug why there's a difference.

We'll learn about tools like the Root Cause Analysis to see where the bug came from.

#### Where We'll Be Looking
* [Applitools Dashboard](https://eyes.applitools.com/app/test-results/)

#### Resources
* [Applitools - Root Cause Analysis](https://applitools.com/root-cause-analysis/)
