## Description

<div><p>A boy named Vasya wants to play an old Russian solitaire called "Accordion". In this solitaire, the player must observe the following rules:</p><ul> <li> A deck of <span class="tex-span"><i>n</i></span> cards is carefully shuffled, then all <span class="tex-span"><i>n</i></span> cards are put on the table in a line from left to right; </li><li> Before each move the table has several piles of cards lying in a line (initially there are <span class="tex-span"><i>n</i></span> piles, each pile has one card). Let's number the piles from left to right, from 1 to <span class="tex-span"><i>x</i></span>. During one move, a player can take the whole pile with the maximum number <span class="tex-span"><i>x</i></span> (that is the rightmost of remaining) and put it on the top of pile <span class="tex-span"><i>x</i> - 1</span> (if it exists) or on the top of pile <span class="tex-span"><i>x</i> - 3</span> (if it exists). The player can put one pile on top of another one only if the piles' top cards have the same suits or values. Please note that if pile <span class="tex-span"><i>x</i></span> goes on top of pile <span class="tex-span"><i>y</i></span>, then the top card of pile <span class="tex-span"><i>x</i></span> becomes the top card of the resulting pile. Also note that each move decreases the total number of piles by 1; </li><li> The solitaire is considered completed if all cards are in the same pile. </li></ul><p>Vasya has already shuffled the cards and put them on the table, help him understand whether completing this solitaire is possible or not. </p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 52)</span> — the number of cards in Vasya's deck. The next line contains <span class="tex-span"><i>n</i></span> space-separated strings <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> describes the <span class="tex-span"><i>i</i></span>-th card on the table. Each string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> consists of exactly two characters, the first one represents the card's value, the second one represents its suit. Cards on the table are numbered from left to right. </p><p>A card's value is specified by one of these characters: "<span class="tex-font-style-tt">2</span>", "<span class="tex-font-style-tt">3</span>", "<span class="tex-font-style-tt">4</span>", "<span class="tex-font-style-tt">5</span>", "<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">7</span>", "<span class="tex-font-style-tt">8</span>", "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">J</span>", "<span class="tex-font-style-tt">Q</span>", "<span class="tex-font-style-tt">K</span>", "<span class="tex-font-style-tt">A</span>". A card's suit is specified by one of these characters: "<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">H</span>", "<span class="tex-font-style-tt">C</span>".</p><p>It is not guaranteed that the deck has all possible cards. Also, the cards in Vasya's deck can repeat.</p></div><div class="output-specification"><p>On a single line print the answer to the problem: string "YES" (without the quotes) if completing the solitaire is possible, string "NO" (without the quotes) otherwise.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 52)</span> — the number of cards in Vasya's deck. The next line contains <span class="tex-span"><i>n</i></span> space-separated strings <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>, where string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> describes the <span class="tex-span"><i>i</i></span>-th card on the table. Each string <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> consists of exactly two characters, the first one represents the card's value, the second one represents its suit. Cards on the table are numbered from left to right. </p><p>A card's value is specified by one of these characters: "<span class="tex-font-style-tt">2</span>", "<span class="tex-font-style-tt">3</span>", "<span class="tex-font-style-tt">4</span>", "<span class="tex-font-style-tt">5</span>", "<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">7</span>", "<span class="tex-font-style-tt">8</span>", "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">J</span>", "<span class="tex-font-style-tt">Q</span>", "<span class="tex-font-style-tt">K</span>", "<span class="tex-font-style-tt">A</span>". A card's suit is specified by one of these characters: "<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">H</span>", "<span class="tex-font-style-tt">C</span>".</p><p>It is not guaranteed that the deck has all possible cards. Also, the cards in Vasya's deck can repeat.</p>

## Output

<p>On a single line print the answer to the problem: string "YES" (without the quotes) if completing the solitaire is possible, string "NO" (without the quotes) otherwise.</p>





```input1
4
2S 2S 2C 2C

```




```input2
2
3S 2C

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample you can act like that: </p><ul> <li> put the 4-th pile on the 1-st one; </li><li> put the 3-rd pile on the 2-nd one; </li><li> put the 2-nd pile on the 1-st one. </li></ul><p>In the second sample there is no way to complete the solitaire.</p>
