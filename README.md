# Memory Game
A clasic card game.

## Game rules

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
Contain classic shuffling card codes as below:
```
  const number = Array.from(Array(count).keys(0))
  for (let index = (number.length - 1); index > 0; index--) {
    let randenIndex = Math.floor(Math.random() * (index + 1));
    [number[index], number[randenIndex]] = [number[randenIndex], number[index]]
  }
```
# 記憶遊戲
這是一個經典的紙牌遊戲。

## 遊戲規則
遊戲開始時所有牌面朝下，玩家輪流翻開兩張牌。
如果兩張牌的號碼相同，則保留牌並獲得 10 分。否則，他們再次將牌面朝下。
當所有的牌都被拿走時，遊戲結束。

## 特色

### 透過MVC架構編碼
這是一個MVC架構練習專案。

所有的函式都被放在三個物件裡面：model、view和controller。目的是編寫低耦合模組。

### 由 GAME_STATE 控制遊戲狀態
總共有以下5個GAME_STATE狀態。所有遊戲狀態都由 5 GAME_STATE 控制。
```
  const GAME_STATE = {
  FirstCardAwaits: "FirstCardAwaits",
  SecondCardAwaits: "SecondCardAwaits",
  CardsMatchFailed: "CardsMatchFailed",
  CardsMatched: "CardsMatched",
  GameFinished: "GameFinished",
  }
```
### 洗牌編碼
此練習包含以下經典的洗牌編碼：
```
  const number = Array.from(Array(count).keys(0))
  for (let index = (number.length - 1); index > 0; index--) {
    let randenIndex = Math.floor(Math.random() * (index + 1));
    [number[index], number[randenIndex]] = [number[randenIndex], number[index]]
  }
```
