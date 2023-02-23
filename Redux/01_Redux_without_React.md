# Redux API

```js
  compose
  applyMiddleware
  bindActionCreators
  combineReducers
  createStore
```

## compose

it's just a helper function. compose takes a series of functions as arguments and returns a new function that applies each those functions from right-to-left (or, from last-to-first if you're like me and have trouble discerning right from left)

```js
const makeLouder = (string) => string.toUpperCase();
const repeatThreeTimes = (string) => string.repeat(3);
const embolden = (string) => string.bold();


embolden(repeatThreeTimes(makeLouder("hello")));

const makeLouderAndBoldAndRepeatThreeTimes = (string) =>
  embolden(repeatThreeTimes(makeLouder(string)));


const makeLouderAndBoldAndRepeatThreeTimes = redux.compose(
  embolden,
  repeatThreeTimes,
  makeLouder
);
```
