# Lesson 1: Visual Testing

Typical testing includes using code to programmatically make sure things are working as expected. When testing against front end UIs, that includes looking at the rendered HTML and verifying that triggering actions on that HTML works.

But we're missing one big things—we're not testing how people actually SEE our front end UIs. That means our tests can say they pass but our visitors and potential customers might not be able to actually do anything! 😱

With visual testing, we can give our tests vision, making sure we're actually looking at our websites and applications just like our visitors would.

## Getting Started

## Objectives
* Learn about visual testing

## Exercises

### 1. Learn how visual testing works

> Visual testing evaluates the visible output of an application and compares that output against the results expected by design.

_via <https://applitools.com/blog/visual-testing/>_

The gist of this is we can use screenshots to compare how our application looks over time. Once we have a baseline (our first or most recently approved screenshot), we can make sure every time we run our test, we can compare the current state of our application to that screenshot.

And this doesn't just apply to an entire application, but [individual components](https://applitools.com/tutorials/storybook-csf-react.html) as well!

We'll take a quick look at how visual testing works and what to expect to accomplish in this workshop.

#### Resources
* [What Is Visual Testing?](https://applitools.com/blog/visual-testing/)