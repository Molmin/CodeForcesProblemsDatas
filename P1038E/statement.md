## Description

<div><p>You are given $n$ blocks, each of them is of the form <span class="tex-font-style-tt">[color$_1$|value|color$_2$]</span>, where the block can also be flipped to get <span class="tex-font-style-tt">[color$_2$|value|color$_1$]</span>. </p><p>A sequence of blocks is called <span class="tex-font-style-it">valid</span> if the touching endpoints of neighboring blocks have the same color. For example, the sequence of three blocks A, B and C is valid if the left color of the B is the same as the right color of the A and the right color of the B is the same as the left color of C.</p><p>The value of the sequence is defined as the sum of the values of the blocks in this sequence.</p><p>Find the maximum possible value of the valid sequence that can be constructed from the subset of the given blocks. The blocks from the subset can be reordered and flipped if necessary. Each block can be used at most once in the sequence.</p></div><div class="input-specification"><p>The first line of input contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of given blocks.</p><p>Each of the following $n$ lines describes corresponding block and consists of $\mathrm{color}_{1,i}$, $\mathrm{value}_i$ and $\mathrm{color}_{2,i}$ ($1 \le \mathrm{color}_{1,i}, \mathrm{color}_{2,i} \le 4$, $1 \le \mathrm{value}_i \le 100\,000$).</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the maximum total value of the subset of blocks, which makes a valid sequence.</p></div>

## Input

<p>The first line of input contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of given blocks.</p><p>Each of the following $n$ lines describes corresponding block and consists of $\mathrm{color}_{1,i}$, $\mathrm{value}_i$ and $\mathrm{color}_{2,i}$ ($1 \le \mathrm{color}_{1,i}, \mathrm{color}_{2,i} \le 4$, $1 \le \mathrm{value}_i \le 100\,000$).</p>

## Output

<p>Print exactly one integer&nbsp;— the maximum total value of the subset of blocks, which makes a valid sequence.</p>





```input1
6
2 1 4
1 2 4
3 4 4
2 8 3
3 16 3
1 32 2

```




```input2
7
1 100000 1
1 100000 2
1 100000 2
4 50000 3
3 50000 4
4 50000 4
3 50000 3

```




```input3
4
1 1000 1
2 500 2
3 250 3
4 125 4

```




```output1
63
```




```output2
300000
```




```output3
1000
```



## Note

<p>In the first example, it is possible to form a valid sequence from all blocks.</p><p>One of the valid sequences is the following:</p><p><span class="tex-font-style-tt">[4|2|1]</span> <span class="tex-font-style-tt">[1|32|2]</span> <span class="tex-font-style-tt">[2|8|3]</span> <span class="tex-font-style-tt">[3|16|3]</span> <span class="tex-font-style-tt">[3|4|4]</span> <span class="tex-font-style-tt">[4|1|2]</span></p><p>The first block from the input (<span class="tex-font-style-tt">[2|1|4]</span> $\to$ <span class="tex-font-style-tt">[4|1|2]</span>) and second (<span class="tex-font-style-tt">[1|2|4]</span> $\to$ <span class="tex-font-style-tt">[4|2|1]</span>) are flipped.</p><p>In the second example, the optimal answers can be formed from the first three blocks as in the following (the second or the third block from the input is flipped):</p><p><span class="tex-font-style-tt">[2|100000|1]</span> <span class="tex-font-style-tt">[1|100000|1]</span> <span class="tex-font-style-tt">[1|100000|2]</span></p><p>In the third example, it is not possible to form a valid sequence of two or more blocks, so the answer is a sequence consisting only of the first block since it is the block with the largest value.</p>
