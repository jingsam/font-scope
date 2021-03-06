# font-scope

[![build status](https://secure.travis-ci.org/mapbox/font-scope.png)](http://travis-ci.org/mapbox/font-scope)

generate font debugging information


### `fontScope(points_array)`

Analyze a font's coverage across languages

Analysis results include:

```js
{
  name: 'English',    // English font name
  id: 'en',           // Unicode font code
  coverages: [26, 0], // array of how many codepoints are covered by each points
  count: 26,          // codepoints in this font for this language
  total: 26           // codepoints in this language
}
```


### Parameters

| parameter      | type             | description                                                                        |
| -------------- | ---------------- | ---------------------------------------------------------------------------------- |
| `points_array` | Array\.\<Array\> | an array of arrays of codepoints, corresponding to the coverage of multiple fonts. |



**Returns** `Object`, analysis

## Installation

Requires [nodejs](http://nodejs.org/).

```sh
$ npm install font-scope
```

## Tests

```sh
$ npm test
```


