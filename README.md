# Memory Game
A clasic card game.
The game starts with all the cards face down and players take turns to turn over two cards. 
If the two cards have the same number, then they keep the cards and get 10 points. Otherwise, they turn the cards face down again. 
The game completes when all the cards have been taken.

## Features

### Coding by MVC Structure.
It is a MVC structure practice program. 
All moudules are classified into three objects: model, view and controller. The target is to write low coupling modules.

### Progress Controlled by GAME_STATE
The program is devided into following 5 GAME_STATE. All processes are controled by the 5 GAME_STATE.
```
  const GAME_STATE = {
  FirstCardAwaits: "FirstCardAwaits",
  SecondCardAwaits: "SecondCardAwaits",
  CardsMatchFailed: "CardsMatchFailed",
  CardsMatched: "CardsMatched",
  GameFinished: "GameFinished",
  }
```
### Shuffling Card Codes
Contain clastic shuffling card codes as below:
```
  const number = Array.from(Array(count).keys(0))
  for (let index = (number.length - 1); index > 0; index--) {
    let randenIndex = Math.floor(Math.random() * (index + 1));
    [number[index], number[randenIndex]] = [number[randenIndex], number[index]]
  }
```
