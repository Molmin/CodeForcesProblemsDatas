## Description

<div><p>Karen just got home from the supermarket, and is getting ready to go to sleep.</p><center> <img class="tex-graphics" src="file://ZH2IFcB9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After taking a shower and changing into her pajamas, she looked at her shelf and saw an album. Curious, she opened it and saw a trading card collection.</p><p>She recalled that she used to play with those cards as a child, and, although she is now grown-up, she still wonders a few things about it.</p><p>Each card has three characteristics: <span class="tex-font-style-it">strength</span>, <span class="tex-font-style-it">defense</span> and <span class="tex-font-style-it">speed</span>. The values of all characteristics of all cards are positive integers. The maximum possible strength any card can have is <span class="tex-span"><i>p</i></span>, the maximum possible defense is <span class="tex-span"><i>q</i></span> and the maximum possible speed is <span class="tex-span"><i>r</i></span>.</p><p>There are <span class="tex-span"><i>n</i></span> cards in her collection. The <span class="tex-span"><i>i</i></span>-th card has a strength <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, defense <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and speed <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, respectively.</p><p>A card <span class="tex-font-style-it">beats</span> another card if at least two of its characteristics are <span class="tex-font-style-it">strictly greater</span> than the corresponding characteristics of the other card.</p><p>She now wonders how many different cards can beat all the cards in her collection. Two cards are considered different if at least one of their characteristics have different values.</p></div><div class="input-specification"><p>The first line of input contains four integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>p</i>, <i>q</i>, <i>r</i> ≤ 500000</span>), the number of cards in the collection, the maximum possible strength, the maximum possible defense, and the maximum possible speed, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain three integers. In particular, the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i></span>), the strength, defense and speed of the <span class="tex-span"><i>i</i></span>-th collection card, respectively.</p></div><div class="output-specification"><p>Output a single integer on a line by itself, the number of different cards that can beat all the cards in her collection.</p></div>

## Input

<p>The first line of input contains four integers, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>p</i>, <i>q</i>, <i>r</i> ≤ 500000</span>), the number of cards in the collection, the maximum possible strength, the maximum possible defense, and the maximum possible speed, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines each contain three integers. In particular, the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>p</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>q</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i></span>), the strength, defense and speed of the <span class="tex-span"><i>i</i></span>-th collection card, respectively.</p>

## Output

<p>Output a single integer on a line by itself, the number of different cards that can beat all the cards in her collection.</p>





```input1
3 4 4 5
2 2 5
1 3 4
4 1 1

```




```input2
5 10 10 10
1 1 1
1 1 1
1 1 1
1 1 1
1 1 1

```




```output1
10

```




```output2
972

```



## Note

<p>In the first test case, the maximum possible strength is <span class="tex-span">4</span>, the maximum possible defense is <span class="tex-span">4</span> and the maximum possible speed is <span class="tex-span">5</span>. Karen has three cards:</p><ul> <li> The first card has strength <span class="tex-span">2</span>, defense <span class="tex-span">2</span> and speed <span class="tex-span">5</span>. </li><li> The second card has strength <span class="tex-span">1</span>, defense <span class="tex-span">3</span> and speed <span class="tex-span">4</span>. </li><li> The third card has strength <span class="tex-span">4</span>, defense <span class="tex-span">1</span> and speed <span class="tex-span">1</span>. </li></ul><p>There are <span class="tex-span">10</span> cards that beat all the cards here:</p><ol> <li> The card with strength <span class="tex-span">3</span>, defense <span class="tex-span">3</span> and speed <span class="tex-span">5</span>. </li><li> The card with strength <span class="tex-span">3</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">2</span>. </li><li> The card with strength <span class="tex-span">3</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">3</span>. </li><li> The card with strength <span class="tex-span">3</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">4</span>. </li><li> The card with strength <span class="tex-span">3</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">5</span>. </li><li> The card with strength <span class="tex-span">4</span>, defense <span class="tex-span">3</span> and speed <span class="tex-span">5</span>. </li><li> The card with strength <span class="tex-span">4</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">2</span>. </li><li> The card with strength <span class="tex-span">4</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">3</span>. </li><li> The card with strength <span class="tex-span">4</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">4</span>. </li><li> The card with strength <span class="tex-span">4</span>, defense <span class="tex-span">4</span> and speed <span class="tex-span">5</span>. </li></ol><p>In the second test case, the maximum possible strength is <span class="tex-span">10</span>, the maximum possible defense is <span class="tex-span">10</span> and the maximum possible speed is <span class="tex-span">10</span>. Karen has five cards, all with strength <span class="tex-span">1</span>, defense <span class="tex-span">1</span> and speed <span class="tex-span">1</span>.</p><p>Any of the <span class="tex-span">972</span> cards which have at least two characteristics greater than <span class="tex-span">1</span> can beat all of the cards in her collection.</p>
