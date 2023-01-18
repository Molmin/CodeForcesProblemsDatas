## Description

<div><p>Ann and Borya have <span class="tex-span"><i>n</i></span> piles with candies and <span class="tex-span"><i>n</i></span> is even number. There are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> candies in pile with number <span class="tex-span"><i>i</i></span>.</p><p>Ann likes numbers which are square of some integer and Borya doesn't like numbers which are square of any integer. During one move guys can select some pile with candies and add one candy to it (this candy is new and doesn't belong to any other pile) or remove one candy (if there is at least one candy in this pile). </p><p>Find out minimal number of moves that is required to make exactly <span class="tex-span"><i>n</i> / 2</span> piles contain number of candies that is a square of some integer and exactly <span class="tex-span"><i>n</i> / 2</span> piles contain number of candies that is not a square of any integer.</p></div><div class="input-specification"><p>First line contains one <span class="tex-font-style-bf">even</span> integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— number of piles with candies.</p><p>Second line contains sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— amounts of candies in each pile.</p></div><div class="output-specification"><p>Output minimal number of steps required to make exactly <span class="tex-span"><i>n</i> / 2</span> piles contain number of candies that is a square of some integer and exactly <span class="tex-span"><i>n</i> / 2</span> piles contain number of candies that is not a square of any integer. If condition is already satisfied output <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>First line contains one <span class="tex-font-style-bf">even</span> integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— number of piles with candies.</p><p>Second line contains sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— amounts of candies in each pile.</p>

## Output

<p>Output minimal number of steps required to make exactly <span class="tex-span"><i>n</i> / 2</span> piles contain number of candies that is a square of some integer and exactly <span class="tex-span"><i>n</i> / 2</span> piles contain number of candies that is not a square of any integer. If condition is already satisfied output <span class="tex-font-style-tt">0</span>.</p>





```input1
4
12 14 30 4

```




```input2
6
0 0 0 0 0 0

```




```input3
6
120 110 23 34 25 45

```




```input4
10
121 56 78 81 45 100 1 0 54 78

```




```output1
2

```




```output2
6

```




```output3
3

```




```output4
0

```



## Note

<p>In first example you can satisfy condition in two moves. During each move you should add one candy to second pile. After it size of second pile becomes <span class="tex-span">16</span>. After that Borya and Ann will have two piles with number of candies which is a square of integer (second and fourth pile) and two piles with number of candies which is not a square of any integer (first and third pile).</p><p>In second example you should add two candies to any three piles.</p>
