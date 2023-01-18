## Description

<div><p>In late autumn evening <span class="tex-span"><i>n</i></span> robots gathered in the cheerful company of friends. Each robot has a unique identifier&nbsp;— an integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>At some moment, robots decided to play the game "Snowball". Below there are the rules of this game. First, all robots stand in a row. Then the first robot says his identifier. After that the second robot says the identifier of the first robot and then says his own identifier. Then the third robot says the identifier of the first robot, then says the identifier of the second robot and after that says his own. This process continues from left to right until the <span class="tex-span"><i>n</i></span>-th robot says his identifier.</p><p>Your task is to determine the <span class="tex-span"><i>k</i></span>-th identifier to be pronounced.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(2·10<sup class="upper-index">9</sup>, <i>n</i>·(<i>n</i> + 1) / 2</span>).</p><p>The second line contains the sequence <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— identifiers of roborts. It is guaranteed that all identifiers are different.</p></div><div class="output-specification"><p>Print the <span class="tex-span"><i>k</i></span>-th pronounced identifier (assume that the numeration starts from <span class="tex-span">1</span>).</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(2·10<sup class="upper-index">9</sup>, <i>n</i>·(<i>n</i> + 1) / 2</span>).</p><p>The second line contains the sequence <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— identifiers of roborts. It is guaranteed that all identifiers are different.</p>

## Output

<p>Print the <span class="tex-span"><i>k</i></span>-th pronounced identifier (assume that the numeration starts from <span class="tex-span">1</span>).</p>





```input1
2 2
1 2

```




```input2
4 5
10 4 18 3

```




```output1
1

```




```output2
4

```



## Note

<p>In the first sample identifiers of robots will be pronounced in the following order: <span class="tex-span">1</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>. As <span class="tex-span"><i>k</i> = 2</span>, the answer equals to <span class="tex-span">1</span>.</p><p>In the second test case identifiers of robots will be pronounced in the following order: <span class="tex-span">10</span>, <span class="tex-span">10</span>, <span class="tex-span">4</span>, <span class="tex-span">10</span>, <span class="tex-span">4</span>, <span class="tex-span">18</span>, <span class="tex-span">10</span>, <span class="tex-span">4</span>, <span class="tex-span">18</span>, <span class="tex-span">3</span>. As <span class="tex-span"><i>k</i> = 5</span>, the answer equals to <span class="tex-span">4</span>.</p>
