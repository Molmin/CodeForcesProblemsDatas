## Description

<div><p>Little Petya likes to play a lot. Most of all he likes to play a game «Holes». This is a game for one person with following rules:</p><p>There are <span class="tex-span"><i>N</i></span> holes located in a single row and numbered from left to right with numbers from 1 to <span class="tex-span"><i>N</i></span>. Each hole has it's own power (hole number <span class="tex-span"><i>i</i></span> has the power <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>). If you throw a ball into hole <span class="tex-span"><i>i</i></span> it will immediately jump to hole <span class="tex-span"><i>i</i> + <i>a</i><sub class="lower-index"><i>i</i></sub></span>, then it will jump out of it and so on. If there is no hole with such number, the ball will just jump out of the row. On each of the <span class="tex-span"><i>M</i></span> moves the player can perform one of two actions: </p><ul> <li> Set the power of the hole <span class="tex-span"><i>a</i></span> to value <span class="tex-span"><i>b</i></span>. </li><li> Throw a ball into the hole <span class="tex-span"><i>a</i></span> and count the number of jumps of a ball before it jump out of the row and also write down the number of the hole from which it jumped out just before leaving the row. </li></ul><p>Petya is not good at math, so, as you have already guessed, you are to perform all computations.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>M</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of holes in a row and the number of moves. The second line contains <span class="tex-span"><i>N</i></span> positive integers not exceeding <span class="tex-span"><i>N</i></span> — initial values of holes power. The following <span class="tex-span"><i>M</i></span> lines describe moves made by Petya. Each of these line can be one of the two types: </p><ul> <li> <span class="tex-span">0</span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> </li><li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i></span> </li></ul> Type <span class="tex-span">0</span> means that it is required to set the power of hole <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>, and type <span class="tex-span">1</span> means that it is required to throw a ball into the <span class="tex-span"><i>a</i></span>-th hole. Numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are positive integers do not exceeding <span class="tex-span"><i>N</i></span>.</div><div class="output-specification"><p>For each move of the type <span class="tex-span">1</span> output two space-separated numbers on a separate line — the number of the last hole the ball visited before leaving the row and the number of jumps it made.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>M</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of holes in a row and the number of moves. The second line contains <span class="tex-span"><i>N</i></span> positive integers not exceeding <span class="tex-span"><i>N</i></span> — initial values of holes power. The following <span class="tex-span"><i>M</i></span> lines describe moves made by Petya. Each of these line can be one of the two types: </p><ul> <li> <span class="tex-span">0</span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> </li><li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i></span> </li></ul> Type <span class="tex-span">0</span> means that it is required to set the power of hole <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>, and type <span class="tex-span">1</span> means that it is required to throw a ball into the <span class="tex-span"><i>a</i></span>-th hole. Numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are positive integers do not exceeding <span class="tex-span"><i>N</i></span>.

## Output

<p>For each move of the type <span class="tex-span">1</span> output two space-separated numbers on a separate line — the number of the last hole the ball visited before leaving the row and the number of jumps it made.</p>





```input1
8 5
1 1 1 1 1 2 8 2
1 1
0 1 3
1 1
0 3 4
1 2

```




```output1
8 7
8 5
7 3

```


