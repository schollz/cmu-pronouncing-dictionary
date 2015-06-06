# cmu-pronouncing-dictionary

All the 134,000+ words in the CMU pronouncing dictionary as a simple JSON object

> The CMU Pronouncing Dictionary (also known as cmudict) is a public domain pronouncing dictionary created by Carnegie Mellon University (CMU). It defines a mapping from English words to their North American pronunciations, and is commonly used in speech processing applications

There are a handful of npm modules for working with the [CMU pronouncing dictionary](http://www.speech.cs.cmu.edu/cgi-bin/cmudict), but none so simple as this one. Unlike the [alternatives](https://www.npmjs.com/search?q=cmu), this module simple exports an object containing words as keys and their Arpabet transcriptions as values. Here's a sample:

```json
{
  "allergen": "AE1 L ER0 JH AH0 N",
  "allergens": "AE1 L ER0 JH AH0 N Z",
  "allergic": "AH0 L ER1 JH IH0 K",
  "allergies": "AE1 L ER0 JH IY0 Z",
  "allergist": "AE1 L ER0 JH AH0 S T",
  "allergist's": "AE1 L ER0 JH AH0 S T S",
  "allergist's(1)": "AE1 L ER0 JH AH0 S",
  "allergists": "AE1 L ER0 JH AH0 S T S",
  "allergists(1)": "AE1 L ER0 JH AH0 S",
  "allergy": "AE1 L ER0 JH IY0",
  "allers": "AO1 L ER0 Z",
  "allert": "AE1 L ER0 T",
  "allerton": "AE1 L ER0 T AH0 N",
  "alles": "EY1 L Z",
  "alleva": "AA0 L EY1 V AH0",
  "alleviate": "AH0 L IY1 V IY0 EY2 T",
  "alleviated": "AH0 L IY1 V IY0 EY2 T IH0 D",
  "alleviates": "AH0 L IY1 V IY0 EY0 T S",
  "alleviating": "AH0 L IY1 V IY0 EY2 T IH0 NG"
}
```

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install cmu-pronouncing-dictionary --save
```

## Usage

```js
const words = require('cmu-pronouncing-dictionary')

words.length
// => 133779

words.phenomenon
// => 'F AH0 N AA1 M AH0 N AA2 N'
words.zygote
// => 'Z AY1 G OW0 T'
```

## Tests

```sh
npm install
npm test
```

## Dependencies

None

## Dev Dependencies

- [code](https://github.com/hapijs/code): assertion library
- [mocha](https://github.com/mochajs/mocha): simple, flexible, fun test framework
- [standard](https://github.com/feross/standard): JavaScript Standard Style

## License

ISC

_Generated by [package-json-to-readme](https://github.com/zeke/package-json-to-readme)_
