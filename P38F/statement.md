## Description

<div><p>Once Petya and Vasya invented a new game and called it "Smart Boy". They located a certain set of words — the dictionary — for the game. It is admissible for the dictionary to contain similar words. </p><p>The rules of the game are as follows: first the first player chooses any letter (a word as long as <span class="tex-span">1</span>) from any word from the dictionary and writes it down on a piece of paper. The second player adds some other letter to this one's initial or final position, thus making a word as long as <span class="tex-span">2</span>, then it's the first player's turn again, he adds a letter in the beginning or in the end thus making a word as long as <span class="tex-span">3</span> and so on. But the player mustn't break one condition: the newly created word must be a substring of a word from a dictionary. The player who can't add a letter to the current word without breaking the condition loses.</p><p>Also if by the end of a turn a certain string <span class="tex-span"><i>s</i></span> is written on paper, then the player, whose turn it just has been, gets a number of points according to the formula:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://XsPk1PZf.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>where </p><ul> <li> <img align="middle" class="tex-formula" src="file://rAVuYJUR.png" style="max-width: 100.0%;max-height: 100.0%;"> is a sequence number of symbol <span class="tex-span"><i>c</i></span> in Latin alphabet, numbered starting from <span class="tex-span">1</span>. For example, <img align="middle" class="tex-formula" src="file://xzJWFfti.png" style="max-width: 100.0%;max-height: 100.0%;">, and <img align="middle" class="tex-formula" src="file://5bcSjxap.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> <img align="middle" class="tex-formula" src="file://GHdkctMk.png" style="max-width: 100.0%;max-height: 100.0%;"> is the number of words from the dictionary where the line <span class="tex-span"><i>s</i></span> occurs as a substring at least once. </li></ul><p>Your task is to learn who will win the game and what the final score will be. Every player plays optimally and most of all tries to win, then — to maximize the number of his points, then — to minimize the number of the points of the opponent.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> which is the number of words in the located dictionary <span class="tex-span">(1 ≤ <i>n</i> ≤ 30)</span>. The <span class="tex-span"><i>n</i></span> lines contain the words from the dictionary — one word is written on one line. Those lines are nonempty, consisting of Latin lower-case characters no longer than <span class="tex-span">30</span> characters. Equal words can be in the list of words.</p></div><div class="output-specification"><p>On the first output line print a line "First" or "Second" which means who will win the game. On the second line output the number of points of the first player and the number of points of the second player after the game ends. Separate the numbers by a single space.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> which is the number of words in the located dictionary <span class="tex-span">(1 ≤ <i>n</i> ≤ 30)</span>. The <span class="tex-span"><i>n</i></span> lines contain the words from the dictionary — one word is written on one line. Those lines are nonempty, consisting of Latin lower-case characters no longer than <span class="tex-span">30</span> characters. Equal words can be in the list of words.</p>

## Output

<p>On the first output line print a line "First" or "Second" which means who will win the game. On the second line output the number of points of the first player and the number of points of the second player after the game ends. Separate the numbers by a single space.</p>





```input1
2
aba
abac

```




```input2
3
artem
nik
max

```




```output1
Second
29 35

```




```output2
First
2403 1882

```


