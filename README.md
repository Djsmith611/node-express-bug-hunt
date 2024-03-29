# Node & Express Bug Hunt!

**READ ALL INSTRUCTIONS BEFORE STARTING**

There are 10 bugs in total, can you find them all? There are hints throughout (???), you should only need to make minor modifcations to 10 lines of code.

**Don't race through the files looking for the issues!** They should all have a console log or error that help you identify them. Read the console so that you know what error will cause each bug. The last one is tricky since it doesn't throw any errors. Document the error, line number and your fix in this README for each of the bugs.

## Setup
```
npm install
npm start
```

> NOTE: A couple of bugs prevent the server from starting.

## Error List

TODO: Add the error here followed by the line of code you fixed.

### Bug 0

`ReferenceError: app is not defined`

Fixed `quote.router.js` line 28: switch `app` to `router`. _This is the solution to the first bug._

### Bug 1
`TypeError: Router.use() requires a middleware function but got a Object`

Fixed `quote.router.js` line 33: Added `module.exports = router;`.

### Bug 2
`Cannot GET /` `Failed to load resource: the server responded with a status of 404 (Not Found)`

Fixed `server.js` line 18: changed `server` to `server/public`.

### Bug 3
`GET http://localhost:5007/quotes 404 (Not Found)`

Fixed `client.js` line 7: Changed `/quotes}` to `/quotes`.

### Bug 4
`GET http://localhost:5007/quotes%7D 404 (Not Found)`

Fixed `quote.router.js` line 10: changed `/quotes` to `/`.

### Bug 5
`TypeError: quotesFromServer is not iterable`

Fixed `quote.router.js` line 6: changed `{}` to `[]`.

### Bug 6
`POST http://localhost:5007/quotes 500 (Internal Server Error)`

Fixed `quote.router.js` line 24: changed `quotesList.push` to `quoteList.push`.

### Bug 7
`ReferenceError: getQuote is not defined`

Fixed `client.js` line 52: changed `getQuote` to `getQuotes`.

### Bug 8
No `DOCTYPE` attribute.
Fixed `index.html` line 1: added `DOCTYPE` attribute.

### Bug 9
`client.js` line 24 and 16: commented out `i` as it had no function.

### Bug 10
`quote.router.js` line 11: added `res.status(200)` to set the status to OK.



## Extra Practice (Optional)

Complete the JS debugging exercises at:

- https://education.launchcode.org/intro-to-professional-web-dev/chapters/errors-and-debugging/exercises.html
