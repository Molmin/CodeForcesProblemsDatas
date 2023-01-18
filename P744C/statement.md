## Description

<div><p>One day, Hongcow goes to the store and sees a brand new deck of <span class="tex-span"><i>n</i></span> special cards. Each individual card is either red or blue. He decides he wants to buy them immediately. To do this, he needs to play a game with the owner of the store.</p><p>This game takes some number of turns to complete. On a turn, Hongcow may do one of two things: </p><ul> <li> Collect tokens. Hongcow collects <span class="tex-span">1</span> red token <span class="tex-font-style-bf">and</span> <span class="tex-span">1</span> blue token by choosing this option (thus, <span class="tex-span">2</span> tokens in total per one operation). </li><li> Buy a card. Hongcow chooses some card and spends tokens to purchase it as specified below. </li></ul><p>The <span class="tex-span"><i>i</i></span>-th card requires <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> red resources and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> blue resources. Suppose Hongcow currently has <span class="tex-span"><i>A</i></span> red cards and <span class="tex-span"><i>B</i></span> blue cards. Then, the <span class="tex-span"><i>i</i></span>-th card will require Hongcow to spend <span class="tex-span"><i>max</i>(<i>r</i><sub class="lower-index"><i>i</i></sub> - <i>A</i>, 0)</span> red tokens, and <span class="tex-span"><i>max</i>(<i>b</i><sub class="lower-index"><i>i</i></sub> - <i>B</i>, 0)</span> blue tokens. Note, only tokens disappear, but the cards stay with Hongcow forever. Each card can be bought only once.</p><p>Given a description of the cards and their costs determine the minimum number of turns Hongcow needs to purchase all cards.</p></div><div class="input-specification"><p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines of input will contain three tokens <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> will be '<span class="tex-font-style-tt">R</span>' or '<span class="tex-font-style-tt">B</span>', denoting the color of the card as red or blue. <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> will be an integer denoting the amount of red resources required to obtain the card, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will be an integer denoting the amount of blue resources required to obtain the card (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Output a single integer, denoting the minimum number of turns needed to acquire all the cards.</p></div>

## Input

<p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines of input will contain three tokens <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> will be '<span class="tex-font-style-tt">R</span>' or '<span class="tex-font-style-tt">B</span>', denoting the color of the card as red or blue. <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> will be an integer denoting the amount of red resources required to obtain the card, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will be an integer denoting the amount of blue resources required to obtain the card (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Output a single integer, denoting the minimum number of turns needed to acquire all the cards.</p>





```input1
3
R 0 1
B 1 0
R 1 1

```




```input2
3
R 3 0
R 2 0
R 1 0

```




```output1
4

```




```output2
6

```



## Note

<p>For the first sample, Hongcow's four moves are as follows: </p><ol> <li> Collect tokens </li><li> Buy card <span class="tex-span">1</span> </li><li> Buy card <span class="tex-span">2</span> </li><li> Buy card <span class="tex-span">3</span> </li></ol> Note, at the fourth step, Hongcow is able to buy card <span class="tex-span">3</span> because Hongcow already has one red and one blue card, so we don't need to collect tokens.<p>For the second sample, one optimal strategy is as follows: </p><ol> <li> Collect tokens </li><li> Collect tokens </li><li> Buy card <span class="tex-span">2</span> </li><li> Collect tokens </li><li> Buy card <span class="tex-span">3</span> </li><li> Buy card <span class="tex-span">1</span> </li></ol> At the fifth step, even though Hongcow has a red token, Hongcow doesn't actually need to spend it, since Hongcow has a red card already.
