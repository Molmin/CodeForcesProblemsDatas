## Description

<div><p>Oleg the bank client and Igor the analyst are arguing again. This time, they want to pick a gift as a present for their friend, ZS the coder. After a long thought, they decided that their friend loves to eat carrots the most and thus they want to pick the best carrot as their present.</p><p>There are <span class="tex-span"><i>n</i></span> carrots arranged in a line. The <span class="tex-span"><i>i</i></span>-th carrot from the left has juiciness <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Oleg thinks ZS loves juicy carrots whereas Igor thinks that he hates juicy carrots. Thus, Oleg would like to maximize the juiciness of the carrot they choose while Igor would like to minimize the juiciness of the carrot they choose.</p><p>To settle this issue, they decided to play a game again. Oleg and Igor take turns to play the game. In each turn, a player can choose a carrot from either end of the line, and eat it. The game ends when only one carrot remains. Oleg moves first. The last remaining carrot will be the carrot that they will give their friend, ZS.</p><p>Oleg is a sneaky bank client. When Igor goes to a restroom, he performs <span class="tex-span"><i>k</i></span> moves before the start of the game. Each move is the same as above (eat a carrot from either end of the line). After Igor returns, they start the game with Oleg still going first. </p><p>Oleg wonders: for each <span class="tex-span"><i>k</i></span> such that <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i> - 1</span>, what is the juiciness of the carrot they will give to ZS if he makes <span class="tex-span"><i>k</i></span> extra moves beforehand and both players play optimally?</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the total number of carrots.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the juiciness of the <span class="tex-span"><i>i</i></span>-th carrot from the left of the line.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span>. Here, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> denotes the juiciness of the carrot the friends will present to ZS if <span class="tex-span"><i>k</i> = <i>i</i></span>.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the total number of carrots.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the juiciness of the <span class="tex-span"><i>i</i></span>-th carrot from the left of the line.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i> - 1</sub></span>. Here, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> denotes the juiciness of the carrot the friends will present to ZS if <span class="tex-span"><i>k</i> = <i>i</i></span>.</p>





```input1
4
1 2 3 5

```




```input2
5
1000000000 1000000000 1000000000 1000000000 1

```




```output1
3 3 5 5

```




```output2
1000000000 1000000000 1000000000 1000000000 1000000000

```



## Note

<p>For the first example, </p><p>When <span class="tex-span"><i>k</i> = 0</span>, one possible optimal game is as follows:</p><ul><li> Oleg eats the carrot with juiciness <span class="tex-span">1</span>.</li><li> Igor eats the carrot with juiciness <span class="tex-span">5</span>.</li><li> Oleg eats the carrot with juiciness <span class="tex-span">2</span>.</li><li> The remaining carrot has juiciness <span class="tex-span">3</span>.</li></ul><p>When <span class="tex-span"><i>k</i> = 1</span>, one possible optimal play is as follows:</p><ul><li> Oleg eats the carrot with juiciness <span class="tex-span">1</span> beforehand.</li><li> Oleg eats the carrot with juiciness <span class="tex-span">2</span>.</li><li> Igor eats the carrot with juiciness <span class="tex-span">5</span>.</li><li> The remaining carrot has juiciness <span class="tex-span">3</span>.</li></ul><p>When <span class="tex-span"><i>k</i> = 2</span>, one possible optimal play is as follows:</p><ul><li> Oleg eats the carrot with juiciness <span class="tex-span">1</span> beforehand.</li><li> Oleg eats the carrot with juiciness <span class="tex-span">2</span> beforehand.</li><li> Oleg eats the carrot with juiciness <span class="tex-span">3</span>.</li><li> The remaining carrot has juiciness <span class="tex-span">5</span>.</li></ul><p>When <span class="tex-span"><i>k</i> = 3</span>, one possible optimal play is as follows:</p><ul><li> Oleg eats the carrot with juiciness <span class="tex-span">1</span> beforehand.</li><li> Oleg eats the carrot with juiciness <span class="tex-span">2</span> beforehand.</li><li> Oleg eats the carrot with juiciness <span class="tex-span">3</span> beforehand.</li><li> The remaining carrot has juiciness <span class="tex-span">5</span>.</li></ul><p>Thus, the answer is <span class="tex-span">3, 3, 5, 5</span>.</p><p>For the second sample, Oleg can always eat the carrot with juiciness <span class="tex-span">1</span> since he always moves first. So, the remaining carrot will always have juiciness <span class="tex-span">1000000000</span>.</p>
