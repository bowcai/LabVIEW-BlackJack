# LabVIEW-BlackJack
A LabVIEW program of "[Black Jack](https://en.wikipedia.org/wiki/Blackjack)", 
also known as "Twenty-One (21)".

The program is written in LabVIEW 2018.

### Description

This program is only designed for one player.

This program implements the functions of 
[*Double-Down*](https://en.wikipedia.org/wiki/Blackjack#Player_decisions) 
and [*Insurance*](https://en.wikipedia.org/wiki/Blackjack#Insurance), 
but does not have the functions of 
[*Split*](https://en.wikipedia.org/wiki/Blackjack#Player_decisions)
or [*Surrender*](https://en.wikipedia.org/wiki/Blackjack#Player_decisions).

### Screenshot
<img src="/Images/Screenshot.png" alt="Screenshot" width="70%" height="70%" />

### How to Run
1. Click "Run" on the LabVIEW to execute the program.
2. Set "Number of decks", "Chips in hand", "Bet" and "Blackjack odds" as you wish.
3. Click "Description" button to read the description of program.
4. Click "Deal cards" to start a round, and choose the action in the pop-up window.
5. When a round is over, click "Deal cards" button to start a new round.
6. Click "End the game" to terminate the program.

### Details
The main program [BlackJack.vi](/BlackJack.vi) uses tons of condition structures to determine 
whether Black-Jack, Insurance or Double-Down occurs, so it may seems very 
complicated :(

**The functions of all the sub VIs:**    
- [Draw.vi](/subVIs/Draw.vi) draws a card from the deck, and return one id of the card. 
- [DealerDraw.vi](/subVIs/DealerDraw.vi) is the program for dealer to draw a card.
- [Judge.vi](/subVIs/Judge.vi) compares the value of player's cards and dealer's cards.  
- [Result.vi](/subVIs/Result.vi) shows the result, and calculates the change of chips.  
- [ShowCards.vi](/subVIs/ShowCards.vi) converts the id of card into the image, and shows the image.  
- [ShowCards(Cover).vi](/subVIs/ShowCards(Cover).vi) covers the first card of dealer.  
- [Sum.vi](/subVIs/Sum.vi) sums the value of cards.

The images of cards is downloaded from Wikipedia: https://en.wikipedia.org/wiki/File:Svg-cards-2.0.svg
