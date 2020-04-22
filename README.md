# classic-deck
### A Deck of 52 shuffled Cards and basic methods to get you started in creating card games with JavaScript.

## Installation

Using npm:
```
npm install --save classic-deck
```
In Node.js:
```
const Deck =  require('classic-deck');
```

### Usage:
```
const Deck =  require('classic-deck');
const deck = new Deck();

// deck.show() returns randomly shuffled 52 card deck.
deck.show();  // => [
  '8♥️',  '8♦️',  '3♥️', 'J♣️', '10♠️', '2♥️',
  '6♠️',  '4♠️',  '9♣️', '5♠️', '7♠️',  '2♠️',
  '2♦️',  '3♠️',  '6♦️', 'K♦️', '4♥️',  '5♦️',
  '2♣️',  'K♥️',  'J♥️', '3♣️', '9♠️',  'K♠️',
  '7♥️',  '10♦️', 'Q♠️', '6♣️', '8♠️',  'A♠️',
  '9♦️',  '3♦️',  'Q♥️', 'J♠️', '7♦️',  'J♦️',
  '10♥️', 'Q♣️',  '7♣️', 'A♥️', 'A♣️',  '6♥️',
  '5♥️',  '8♣️',  '5♣️', 'K♣️', '4♣️',  '10♣️',
  '4♦️',  '9♥️',  'A♦️', 'Q♦️'
]


// deck.shuffleDeck() 
Will randomly shuffle remaining cards in the deck.


// deck.discard(x) 
Will discard "x" cards from the top of your deck.
Can use deck.show() to verify the cards have been discarded.


// deck.deal(x)
Will move "x" cards from top of deck
and return them into your hand. Example:

const myHand = deck.deal(7);
console.log(myHand);       // =>
[
  'K♥️',  'Q♦️',
  '10♠️', '7♦️',
  'Q♠️',  '10♥️',
  '7♥️'
]

```