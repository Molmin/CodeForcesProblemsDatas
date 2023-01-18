## Description

<div><p>Two positive integers are coprime if and only if they don't have a common divisor greater than <span class="tex-span">1</span>.</p><p>Some bear doesn't want to tell Radewoosh how to solve some algorithmic problem. So, Radewoosh is going to break into that bear's safe with solutions. To pass through the door, he must enter a permutation of numbers <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. The door opens if and only if an entered permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> satisfies:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://og6z76XB.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In other words, two different elements are coprime if and only if their indices are coprime. </p><p>Some elements of a permutation may be already fixed. In how many ways can Radewoosh fill the remaining gaps so that the door will open? Print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = 0</span> means a gap to fill, and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span> means a fixed number.</p><p>It's guaranteed that if <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>j</i></sub> ≥ 1</span> then <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>Print the number of ways to fill the gaps modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> (i.e. modulo <span class="tex-span">1000000007</span>).</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = 0</span> means a gap to fill, and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span> means a fixed number.</p><p>It's guaranteed that if <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>j</i></sub> ≥ 1</span> then <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>p</i><sub class="lower-index"><i>j</i></sub></span>.</p>

## Output

<p>Print the number of ways to fill the gaps modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> (i.e. modulo <span class="tex-span">1000000007</span>).</p>





```input1
4
0 0 0 0

```




```input2
5
0 0 1 2 0

```




```input3
6
0 0 1 2 0 0

```




```input4
5
5 3 4 2 1

```




```output1
4

```




```output2
2

```




```output3
0

```




```output4
0

```



## Note

<p>In the first sample test, none of four element is fixed. There are four permutations satisfying the given conditions: (1,2,3,4), (1,4,3,2), (3,2,1,4), (3,4,1,2).</p><p>In the second sample test, there must be <span class="tex-span"><i>p</i><sub class="lower-index">3</sub> = 1</span> and <span class="tex-span"><i>p</i><sub class="lower-index">4</sub> = 2</span>. The two permutations satisfying the conditions are: (3,4,1,2,5), (5,4,1,2,3).</p>
