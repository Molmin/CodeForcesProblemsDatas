## Description

<div><p>A game field is a strip of <span class="tex-span">1 × <i>n</i></span> square cells. In some cells there are Packmen, in some cells&nbsp;— asterisks, other cells are empty.</p><p>Packman can move to neighboring cell in <span class="tex-span">1</span> time unit. If there is an asterisk in the target cell then Packman eats it. Packman doesn't spend any time to eat an asterisk.</p><p>In the initial moment of time all Packmen begin to move. Each Packman can change direction of its move unlimited number of times, but it is not allowed to go beyond the boundaries of the game field. Packmen do not interfere with the movement of other packmen; in one cell there can be any number of packmen moving in any directions.</p><p>Your task is to determine minimum possible time after which Packmen can eat all the asterisks.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the game field.</p><p>The second line contains the description of the game field consisting of <span class="tex-span"><i>n</i></span> symbols. If there is symbol '<span class="tex-font-style-tt">.</span>' in position <span class="tex-span"><i>i</i></span> — the cell <span class="tex-span"><i>i</i></span> is empty. If there is symbol '<span class="tex-font-style-tt">*</span>' in position <span class="tex-span"><i>i</i></span> — in the cell <span class="tex-span"><i>i</i></span> contains an asterisk. If there is symbol '<span class="tex-font-style-tt">P</span>' in position <span class="tex-span"><i>i</i></span> — Packman is in the cell <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that on the game field there is at least one Packman and at least one asterisk.</p></div><div class="output-specification"><p>Print minimum possible time after which Packmen can eat all asterisks.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the game field.</p><p>The second line contains the description of the game field consisting of <span class="tex-span"><i>n</i></span> symbols. If there is symbol '<span class="tex-font-style-tt">.</span>' in position <span class="tex-span"><i>i</i></span> — the cell <span class="tex-span"><i>i</i></span> is empty. If there is symbol '<span class="tex-font-style-tt">*</span>' in position <span class="tex-span"><i>i</i></span> — in the cell <span class="tex-span"><i>i</i></span> contains an asterisk. If there is symbol '<span class="tex-font-style-tt">P</span>' in position <span class="tex-span"><i>i</i></span> — Packman is in the cell <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that on the game field there is at least one Packman and at least one asterisk.</p>

## Output

<p>Print minimum possible time after which Packmen can eat all asterisks.</p>





```input1
7
*..P*P*

```




```input2
10
.**PP.*P.*

```




```output1
3

```




```output2
2

```



## Note

<p>In the first example Packman in position <span class="tex-span">4</span> will move to the left and will eat asterisk in position <span class="tex-span">1</span>. He will spend <span class="tex-span">3</span> time units on it. During the same <span class="tex-span">3</span> time units Packman in position <span class="tex-span">6</span> will eat both of neighboring with it asterisks. For example, it can move to the left and eat asterisk in position <span class="tex-span">5</span> (in <span class="tex-span">1</span> time unit) and then move from the position <span class="tex-span">5</span> to the right and eat asterisk in the position <span class="tex-span">7</span> (in <span class="tex-span">2</span> time units). So in <span class="tex-span">3</span> time units Packmen will eat all asterisks on the game field.</p><p>In the second example Packman in the position <span class="tex-span">4</span> will move to the left and after <span class="tex-span">2</span> time units will eat asterisks in positions <span class="tex-span">3</span> and <span class="tex-span">2</span>. Packmen in positions <span class="tex-span">5</span> and <span class="tex-span">8</span> will move to the right and in <span class="tex-span">2</span> time units will eat asterisks in positions <span class="tex-span">7</span> and <span class="tex-span">10</span>, respectively. So <span class="tex-span">2</span> time units is enough for Packmen to eat all asterisks on the game field.</p>
