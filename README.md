## ISICverify - Verify ISIC cards using Node.js
[![Build Status](https://travis-ci.com/GeorgeBgk/isicverify.svg?branch=master)](https://travis-ci.com/GeorgeBgk/isicverify)
### Install
```bash
npm i isicverify
```

### Usage
```js
const verifyISIC = require('isicverify')
verifyISIC('cardnumber').then(function(isValid) {
	console.log(isValid)
})
```

### How it works
ISIC does not have a public API, but they have a [verification form](https://www.isic.org/verify/) which this module fills out and then parses the response HTML to get the result
