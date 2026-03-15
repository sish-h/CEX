# CEX
A lightweight JavaScript library for making cryptocurrency exchange rate queries.

## What it does
CEX allows you to easily retrieve current and historical exchange rates for various cryptocurrencies. It supports multiple exchanges and provides a simple, unified API.

## Installation
To install CEX, run:
```bash
npm install cex-js
```
## Usage
Here's a quick example of how to use CEX:
```javascript
const CEX = require('cex-js');

const cex = new CEX();
cex.getRate('BTC', 'USD')
  .then(rate => console.log(`1 BTC = ${rate} USD`))
  .catch(error => console.error(error));
```
This code creates a new CEX instance and retrieves the current BTC/USD exchange rate.

## Running the tests
If you want to run the tests, you'll need to install the dependencies and then run:
```bash
npm test
```
Make sure you have Node.js and npm installed on your system. That's it! If you have any questions or find a bug, don't hesitate to open an issue.