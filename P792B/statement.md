## Description

<div><p><span class="tex-span"><i>n</i></span> children are standing in a circle and playing the counting-out game. Children are numbered clockwise from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. In the beginning, the first child is considered the leader. The game is played in <span class="tex-span"><i>k</i></span> steps. In the <span class="tex-span"><i>i</i></span>-th step the leader counts out <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> people in clockwise order, starting from the next person. The last one to be pointed at by the leader is eliminated, and the next player after him becomes the new leader.</p><p>For example, if there are children with numbers <span class="tex-span">[8, 10, 13, 14, 16]</span> currently in the circle, the leader is child <span class="tex-span">13</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 12</span>, then counting-out rhyme ends on child <span class="tex-span">16</span>, who is eliminated. Child <span class="tex-span">8</span> becomes the leader.</p><p>You have to write a program which prints the number of the child to be eliminated on every step.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>).</p><p>The next line contains <span class="tex-span"><i>k</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> numbers, the <span class="tex-span"><i>i</i></span>-th one corresponds to the number of child to be eliminated at the <span class="tex-span"><i>i</i></span>-th step.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>).</p><p>The next line contains <span class="tex-span"><i>k</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> numbers, the <span class="tex-span"><i>i</i></span>-th one corresponds to the number of child to be eliminated at the <span class="tex-span"><i>i</i></span>-th step.</p>





```input1
7 5
10 4 11 4 1

```




```input2
3 2
2 5

```




```output1
4 2 5 6 1 

```




```output2
3 2 

```



## Note

<p>Let's consider first example: </p><ul> <li> In the first step child <span class="tex-span">4</span> is eliminated, child <span class="tex-span">5</span> becomes the leader. </li><li> In the second step child <span class="tex-span">2</span> is eliminated, child <span class="tex-span">3</span> becomes the leader. </li><li> In the third step child <span class="tex-span">5</span> is eliminated, child <span class="tex-span">6</span> becomes the leader. </li><li> In the fourth step child <span class="tex-span">6</span> is eliminated, child <span class="tex-span">7</span> becomes the leader. </li><li> In the final step child <span class="tex-span">1</span> is eliminated, child <span class="tex-span">3</span> becomes the leader. </li></ul>
