## Description

<div><p>Fox Ciel is participating in a party in Prime Kingdom. There are <span class="tex-span"><i>n</i></span> foxes there (include Fox Ciel). The i-th fox is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> years old.</p><p>They will have dinner around some round tables. You want to distribute foxes such that:</p><ol> <li> Each fox is sitting at some table. </li><li> Each table has at least 3 foxes sitting around it. </li><li> The sum of ages of any two adjacent foxes around each table should be a prime number. </li></ol><p>If <span class="tex-span"><i>k</i></span> foxes <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>f</i><sub class="lower-index"><i>k</i></sub></span> are sitting around table in clockwise order, then for <span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i> - 1</span>: <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i> + 1</sub></span> are adjacent, and <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>k</i></sub></span> are also adjacent.</p><p>If it is possible to distribute the foxes in the desired manner, find out a way to do that.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 200</span>): the number of foxes in this party. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p></div><div class="output-specification"><p>If it is impossible to do this, output "Impossible".</p><p>Otherwise, in the first line output an integer <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://FOoTWHiH.png" style="max-width: 100.0%;max-height: 100.0%;">): the number of tables.</p><p>Then output <span class="tex-span"><i>m</i></span> lines, each line should start with an integer <span class="tex-span"><i>k</i></span> -=– the number of foxes around that table, and then <span class="tex-span"><i>k</i></span> numbers — indices of fox sitting around that table in clockwise order.</p><p>If there are several possible arrangements, output any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 200</span>): the number of foxes in this party. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p>

## Output

<p>If it is impossible to do this, output "Impossible".</p><p>Otherwise, in the first line output an integer <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://FOoTWHiH.png" style="max-width: 100.0%;max-height: 100.0%;">): the number of tables.</p><p>Then output <span class="tex-span"><i>m</i></span> lines, each line should start with an integer <span class="tex-span"><i>k</i></span> -=– the number of foxes around that table, and then <span class="tex-span"><i>k</i></span> numbers — indices of fox sitting around that table in clockwise order.</p><p>If there are several possible arrangements, output any of them.</p>





```input1
4
3 4 8 9

```




```input2
5
2 2 2 2 2

```




```input3
12
2 3 4 5 6 7 8 9 10 11 12 13

```




```input4
24
2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25

```




```output1
1
4 1 2 4 3

```




```output2
Impossible

```




```output3
1
12 1 2 3 6 5 12 9 8 7 10 11 4

```




```output4
3
6 1 2 3 6 5 4
10 7 8 9 12 15 14 13 16 11 10
8 17 18 23 22 19 20 21 24

```



## Note

<p>In example 1, they can sit around one table, their ages are: 3-8-9-4, adjacent sums are: 11, 17, 13 and 7, all those integers are primes.</p><p>In example 2, it is not possible: the sum of 2+2 = 4 is not a prime number.</p>
