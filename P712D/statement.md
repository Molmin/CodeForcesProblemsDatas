## Description

<div><p>Memory and his friend Lexa are competing to get higher score in one popular computer game. Memory starts with score <span class="tex-span"><i>a</i></span> and Lexa starts with score <span class="tex-span"><i>b</i></span>. In a single turn, both Memory and Lexa get some integer in the range <span class="tex-span">[ - <i>k</i>;<i>k</i>]</span> (i.e. one integer among <span class="tex-span"> - <i>k</i>,  - <i>k</i> + 1,  - <i>k</i> + 2, ...,  - 2,  - 1, 0, 1, 2, ..., <i>k</i> - 1, <i>k</i></span>) and add them to their current scores. The game has exactly <span class="tex-span"><i>t</i></span> turns. Memory and Lexa, however, are not good at this game, so they both always get a random integer at their turn.</p><p>Memory wonders how many possible games exist such that he ends with a strictly higher score than Lexa. Two games are considered to be different if in at least one turn at least one player gets different score. There are <span class="tex-span">(2<i>k</i> + 1)<sup class="upper-index">2<i>t</i></sup></span> games in total. Since the answer can be very large, you should print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Please solve this problem for Memory.</p></div><div class="input-specification"><p>The first and only line of input contains the four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span>, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>)&nbsp;— the amount Memory and Lexa start with, the number <span class="tex-span"><i>k</i></span>, and the number of turns respectively.</p></div><div class="output-specification"><p>Print the number of possible games satisfying the conditions modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>) in one line.</p></div>

## Input

<p>The first and only line of input contains the four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span>, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>)&nbsp;— the amount Memory and Lexa start with, the number <span class="tex-span"><i>k</i></span>, and the number of turns respectively.</p>

## Output

<p>Print the number of possible games satisfying the conditions modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>) in one line.</p>





```input1
1 2 2 1

```




```input2
1 1 1 2

```




```input3
2 12 3 1

```




```output1
6

```




```output2
31

```




```output3
0

```



## Note

<p>In the first sample test, Memory starts with <span class="tex-span">1</span> and Lexa starts with <span class="tex-span">2</span>. If Lexa picks <span class="tex-span"> - 2</span>, Memory can pick <span class="tex-span">0</span>, <span class="tex-span">1</span>, or <span class="tex-span">2</span> to win. If Lexa picks <span class="tex-span"> - 1</span>, Memory can pick <span class="tex-span">1</span> or <span class="tex-span">2</span> to win. If Lexa picks <span class="tex-span">0</span>, Memory can pick <span class="tex-span">2</span> to win. If Lexa picks <span class="tex-span">1</span> or <span class="tex-span">2</span>, Memory cannot win. Thus, there are <span class="tex-span">3 + 2 + 1 = 6</span> possible games in which Memory wins.</p>
