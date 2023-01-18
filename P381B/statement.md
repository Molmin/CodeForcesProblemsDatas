## Description

<div><p>Sereja loves integer sequences very much. He especially likes stairs.</p><p>Sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">|<i>a</i>|</sub></span> (<span class="tex-span">|<i>a</i>|</span> is the length of the sequence) is stairs if there is such index <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ |<i>a</i>|)</span>, that the following condition is met: </p><center class="tex-equation"><span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>i</i> - 1</sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub> &gt; ... &gt; <i>a</i><sub class="lower-index">|<i>a</i>| - 1</sub> &gt; <i>a</i><sub class="lower-index">|<i>a</i>|</sub>.</span></center><p>For example, sequences [1, 2, 3, 2] and [4, 2] are stairs and sequence [3, 1, 2] isn't.</p><p>Sereja has <span class="tex-span"><i>m</i></span> cards with numbers. He wants to put some cards on the table in a row to get a stair sequence. What maximum number of cards can he put on the table?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Sereja's cards. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 5000)</span> — the numbers on the Sereja's cards.</p></div><div class="output-specification"><p>In the first line print the number of cards you can put on the table. In the second line print the resulting stairs.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Sereja's cards. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 5000)</span> — the numbers on the Sereja's cards.</p>

## Output

<p>In the first line print the number of cards you can put on the table. In the second line print the resulting stairs.</p>





```input1
5
1 2 3 4 5

```




```input2
6
1 1 2 2 3 3

```




```output1
5
5 4 3 2 1

```




```output2
5
1 2 3 2 1

```


