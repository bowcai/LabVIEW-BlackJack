# LabVIEW-BlackJack
A LabVIEW program of "Black Jack", also known as "Twenty-One".

The program is written in LabVIEW 2018.

### Description

This program is only designed for one player.

This program implements the functions of *Double-Down* and *Insurance*, but does not have the functions of *Split* or *Surrender*.

### Screenshot
![Screenshot](/Images/Screenshot.png){:height="60%" width="60%"}

### How to Run
1. Click "Run" on the LabVIEW to execute the program.
2. Set "Number of decks", "Chips in hand", "Bet" and "Blackjack odds" as you wish.
3. Click "Description" button to read the description of program.
4. Click "Deal cards" to start a round, and choose the action in the pop-up window.
5. When a round is over, click "Deal cards" button to start a new round.
6. Click "End the game" to terminate the program.

### Introduction to the Program
The main program `BlackJack.vi` uses tons of condition structures to determine 
whether Black-Jack, Insurance or Double-Down occurs, so it may seems very 
complicated :(

The functions of all the sub VIs:  
`DealerDraw.vi` is the program for dealer to draw a card.  
`Draw.vi` draws a card from the deck, and return one id of the card.  
`Judge.vi` compares the value of player's cards and dealer's cards.  
`Result.vi` shows the result, and calculates the change of chips.  
`ShowCards.vi` converts the id of card into the image, and shows the image.  
`ShowCards(Cover).vi` covers the first card of dealer.  
`Sum.vi` sums the value of cards.

The images of poker cards is downloaded from Wikipedia: https://en.wikipedia.org/wiki/File:Svg-cards-2.0.svg
