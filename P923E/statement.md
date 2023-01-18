## Description

<div><p>There is a number <span class="tex-span"><i>x</i></span> initially written on a blackboard. You repeat the following action a fixed amount of times: </p><ol> <li> take the number <span class="tex-span"><i>x</i></span> currently written on a blackboard and erase it </li><li> select an integer uniformly at random from the range <span class="tex-span">[0, <i>x</i>]</span> inclusive, and write it on the blackboard </li></ol><p>Determine the distribution of final number given the distribution of initial number and the number of steps.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the maximum number written on the blackboard&nbsp;— and <span class="tex-span"><i>M</i></span> (<span class="tex-span">0 ≤ <i>M</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of steps to perform.</p><p>The second line contains <span class="tex-span"><i>N</i> + 1</span> integers <span class="tex-span"><i>P</i><sub class="lower-index">0</sub>, <i>P</i><sub class="lower-index">1</sub>, ..., <i>P</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> &lt; 998244353</span>), where <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span> describes the probability that the starting number is <span class="tex-span"><i>i</i></span>. We can express this probability as irreducible fraction <span class="tex-span"><i>P</i> / <i>Q</i></span>, then <img align="middle" class="tex-formula" src="file://WYlMaYgZ.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that the sum of all <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span>s equals <span class="tex-span">1</span> (modulo <span class="tex-span">998244353</span>).</p></div><div class="output-specification"><p>Output a single line of <span class="tex-span"><i>N</i> + 1</span> integers, where <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> is the probability that the final number after <span class="tex-span"><i>M</i></span> steps is <span class="tex-span"><i>i</i></span>. It can be proven that the probability may always be expressed as an irreducible fraction <span class="tex-span"><i>P</i> / <i>Q</i></span>. You are asked to output <img align="middle" class="tex-formula" src="file://ioqaoAYU.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the maximum number written on the blackboard&nbsp;— and <span class="tex-span"><i>M</i></span> (<span class="tex-span">0 ≤ <i>M</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of steps to perform.</p><p>The second line contains <span class="tex-span"><i>N</i> + 1</span> integers <span class="tex-span"><i>P</i><sub class="lower-index">0</sub>, <i>P</i><sub class="lower-index">1</sub>, ..., <i>P</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> &lt; 998244353</span>), where <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span> describes the probability that the starting number is <span class="tex-span"><i>i</i></span>. We can express this probability as irreducible fraction <span class="tex-span"><i>P</i> / <i>Q</i></span>, then <img align="middle" class="tex-formula" src="file://WYlMaYgZ.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that the sum of all <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span>s equals <span class="tex-span">1</span> (modulo <span class="tex-span">998244353</span>).</p>

## Output

<p>Output a single line of <span class="tex-span"><i>N</i> + 1</span> integers, where <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> is the probability that the final number after <span class="tex-span"><i>M</i></span> steps is <span class="tex-span"><i>i</i></span>. It can be proven that the probability may always be expressed as an irreducible fraction <span class="tex-span"><i>P</i> / <i>Q</i></span>. You are asked to output <img align="middle" class="tex-formula" src="file://ioqaoAYU.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 1
0 0 1

```




```input2
2 2
0 0 1

```




```input3
9 350
3 31 314 3141 31415 314159 3141592 31415926 314159265 649178508

```




```output1
332748118 332748118 332748118

```




```output2
942786334 610038216 443664157

```




```output3
822986014 12998613 84959018 728107923 939229297 935516344 27254497 413831286 583600448 442738326

```



## Note

<p>In the first case, we start with number 2. After one step, it will be 0, 1 or 2 with probability 1/3 each.</p><p>In the second case, the number will remain 2 with probability 1/9. With probability 1/9 it stays 2 in the first round and changes to 1 in the next, and with probability 1/6 changes to 1 in the first round and stays in the second. In all other cases the final integer is 0.</p>
