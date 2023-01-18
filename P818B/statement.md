## Description

<div><p><span class="tex-span"><i>n</i></span> children are standing in a circle and playing a game. Children's numbers in clockwise order form a permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>. It is an integer sequence such that each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> appears exactly once in it.</p><p>The game consists of <span class="tex-span"><i>m</i></span> steps. On each step the current leader with index <span class="tex-span"><i>i</i></span> counts out <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> people in clockwise order, starting from the next person. The last one to be pointed at by the leader becomes the new leader.</p><p>You are given numbers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span> — indices of leaders in the beginning of each step. Child with number <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> is the first leader in the game. </p><p>Write a program which will restore a possible permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. If there are multiple solutions then print any of them. If there is no solution then print <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>m</i></span> integer numbers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — indices of leaders in the beginning of each step.</p></div><div class="output-specification"><p>Print such permutation of <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> that leaders in the game will be exactly <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span> if all the rules are followed. If there are multiple solutions print any of them. </p><p>If there is no permutation which satisfies all described conditions print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>m</i></span> integer numbers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — indices of leaders in the beginning of each step.</p>

## Output

<p>Print such permutation of <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> that leaders in the game will be exactly <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>m</i></sub></span> if all the rules are followed. If there are multiple solutions print any of them. </p><p>If there is no permutation which satisfies all described conditions print <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 5
2 3 1 4 4

```




```input2
3 3
3 1 2

```




```output1
3 1 2 4 

```




```output2
-1

```



## Note

<p>Let's follow leadership in the first example: </p><ul> <li> Child <span class="tex-span">2</span> starts. </li><li> Leadership goes from <span class="tex-span">2</span> to <span class="tex-span">2 + <i>a</i><sub class="lower-index">2</sub> = 3</span>. </li><li> Leadership goes from <span class="tex-span">3</span> to <span class="tex-span">3 + <i>a</i><sub class="lower-index">3</sub> = 5</span>. As it's greater than <span class="tex-span">4</span>, it's going in a circle to <span class="tex-span">1</span>. </li><li> Leadership goes from <span class="tex-span">1</span> to <span class="tex-span">1 + <i>a</i><sub class="lower-index">1</sub> = 4</span>. </li><li> Leadership goes from <span class="tex-span">4</span> to <span class="tex-span">4 + <i>a</i><sub class="lower-index">4</sub> = 8</span>. Thus in circle it still remains at <span class="tex-span">4</span>. </li></ul>
