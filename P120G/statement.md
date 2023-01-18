## Description

<div><p>Let's consider the famous game called Boom (aka Hat) with simplified rules.</p><p>There are <span class="tex-span"><i>n</i></span> teams playing the game. Each team has two players. The purpose of the game is to explain the words to the teammate without using any words that contain the same root or that sound similarly. </p><p>Player <span class="tex-span"><i>j</i></span> from team <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>j</i> ≤ 2)</span> is characterized by two numbers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span>. The numbers correspondingly represent the skill of explaining and the skill of understanding this particular player has. </p><p>Besides, <span class="tex-span"><i>m</i></span> cards are used for the game. Each card has a word written on it. The card number <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>m</i>)</span> is characterized by number <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span> — the complexity of the word it contains.</p><p>Before the game starts the cards are put in a deck and shuffled. Then the teams play in turns like that: the 1-st player of the 1-st team, the 1-st player of the 2-nd team, ... , the 1-st player of the <span class="tex-span"><i>n</i></span>-th team, the 2-nd player of the 1-st team, ... , the 2-nd player of the <span class="tex-span"><i>n</i></span>-th team, the 1-st player of the 1-st team and so on.</p><p>Each turn continues for <span class="tex-span"><i>t</i></span> seconds. It goes like that: Initially the time for each turn is <span class="tex-span"><i>t</i></span>. While the time left to a player is more than 0, a player takes a card from the top of the deck and starts explaining the word it has to his teammate. The time needed for the <span class="tex-span"><i>j</i></span>-th player of the <span class="tex-span"><i>i</i></span>-th team to explain the word from the card <span class="tex-span"><i>k</i></span> to his teammate (the <span class="tex-span"><i>q</i></span>-th player of the <span class="tex-span"><i>i</i></span>-th team) equals <span class="tex-span"><i>max</i>(1, <i>c</i><sub class="lower-index"><i>k</i></sub> - (<i>a</i><sub class="lower-index"><i>ij</i></sub> + <i>b</i><sub class="lower-index"><i>iq</i></sub>) - <i>d</i><sub class="lower-index"><i>ik</i></sub>)</span> (if <span class="tex-span"><i>j</i> = 1, </span> then <span class="tex-span"><i>q</i> = 2, </span> else <span class="tex-span"><i>q</i> = 1</span>). The value <span class="tex-span"><i>d</i><sub class="lower-index"><i>ik</i></sub></span> is the number of seconds the <span class="tex-span"><i>i</i></span>-th team has already spent explaining the word <span class="tex-span"><i>k</i></span> during the previous turns. Initially, all <span class="tex-span"><i>d</i><sub class="lower-index"><i>ik</i></sub></span> equal 0. If a team manages to guess the word before the end of the turn, then the time given above is substracted from the duration of the turn, the card containing the guessed word leaves the game, the team wins one point and the game continues. If the team doesn't manage to guess the word, then the card is put at the bottom of the deck, <span class="tex-span"><i>d</i><sub class="lower-index"><i>ik</i></sub></span> increases on the amount of time of the turn, spent on explaining the word. Thus, when this team gets the very same word, they start explaining it not from the beginning, but from the point where they stopped. The game ends when words from all <span class="tex-span"><i>m</i></span> cards are guessed correctly.</p><p>You are given <span class="tex-span"><i>n</i></span> teams and a deck of <span class="tex-span"><i>m</i></span> cards. You should determine for each team, how many points it will have by the end of the game and which words the team will have guessed.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i> ≤ 100)</span>, which correspondingly denote the number of teams and a turn's duration.</p><p>Next <span class="tex-span"><i>n</i></span> lines of the input file contain four integers each: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>b</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, <i>b</i><sub class="lower-index"><i>i</i>2</sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub>, <i>b</i><sub class="lower-index"><i>ij</i></sub> ≤ 100)</span> — the skills of the first and the second player of the <span class="tex-span"><i>i</i></span>-th team. The teams are given in the order in which they play.</p><p>The next line of the input file contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 100)</span> the number of cards.</p><p>Next <span class="tex-span">2<i>m</i></span> lines contain the cards' descriptions. Two lines describe each card. The first line of the description contains the word that consists of no more than 20 characters. The words only contain small Latin letters. The second line of the description contains an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>k</i></sub> ≤ 100</span>) — the complexity of the word written on the <span class="tex-span"><i>k</i></span>-th card. The cards are listed in the order in which the lie in the deck from top to bottom. The words on all cards are different.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th line first print number <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> the number of points the <span class="tex-span"><i>i</i></span>-th team wins. Then print <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> space-separated words — the words from the cards guessed by team <span class="tex-span"><i>i</i></span> in the order in which they were guessed.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i> ≤ 100)</span>, which correspondingly denote the number of teams and a turn's duration.</p><p>Next <span class="tex-span"><i>n</i></span> lines of the input file contain four integers each: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>b</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, <i>b</i><sub class="lower-index"><i>i</i>2</sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub>, <i>b</i><sub class="lower-index"><i>ij</i></sub> ≤ 100)</span> — the skills of the first and the second player of the <span class="tex-span"><i>i</i></span>-th team. The teams are given in the order in which they play.</p><p>The next line of the input file contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 100)</span> the number of cards.</p><p>Next <span class="tex-span">2<i>m</i></span> lines contain the cards' descriptions. Two lines describe each card. The first line of the description contains the word that consists of no more than 20 characters. The words only contain small Latin letters. The second line of the description contains an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>k</i></sub> ≤ 100</span>) — the complexity of the word written on the <span class="tex-span"><i>k</i></span>-th card. The cards are listed in the order in which the lie in the deck from top to bottom. The words on all cards are different.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th line first print number <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> the number of points the <span class="tex-span"><i>i</i></span>-th team wins. Then print <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> space-separated words — the words from the cards guessed by team <span class="tex-span"><i>i</i></span> in the order in which they were guessed.</p>





```input1
2 2
1 1 1 1
1 1 1 1
3
home
1
car
1
brother
1

```




```input2
2 4
1 2 2 1
2 3 2 2
4
armchair
3
quetzalcoatl
10
pilotage
5
defibrillator
7

```




```output1
2 home car 
1 brother 

```




```output2
2 armchair quetzalcoatl 
2 pilotage defibrillator 

```


