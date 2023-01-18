## Description

<div><p>During the break, we decided to relax and play dominoes. Our box with Domino was empty, so we decided to borrow the teacher's dominoes.</p><p>The teacher responded instantly at our request. He put <span class="tex-span"><i>nm</i></span> dominoes on the table as an <span class="tex-span"><i>n</i> × 2<i>m</i></span> rectangle so that each of the <span class="tex-span"><i>n</i></span> rows contained <span class="tex-span"><i>m</i></span> dominoes arranged horizontally. Each half of each domino contained number (0 or 1).</p><p>We were taken aback, and the teacher smiled and said: "Consider some arrangement of dominoes in an <span class="tex-span"><i>n</i> × 2<i>m</i></span> matrix. Let's count for each column of the matrix the sum of numbers in this column. Then among all such sums find the maximum one. Can you rearrange the dominoes in the matrix in such a way that the maximum sum will be minimum possible? Note that it is prohibited to change the orientation of the dominoes, they all need to stay horizontal, nevertheless dominoes are allowed to rotate by 180 degrees. As a reward I will give you all my dominoes".</p><p>We got even more taken aback. And while we are wondering what was going on, help us make an optimal matrix of dominoes.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>).</p><p>In the next lines there is a description of the teachers' matrix. Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> dominoes. The description of one domino is two integers (0 or 1), written without a space — the digits on the left and right half of the domino.</p></div><div class="output-specification"><p>Print the resulting matrix of dominoes in the format: <span class="tex-span"><i>n</i></span> lines, each of them contains <span class="tex-span"><i>m</i></span> space-separated dominoes.</p><p>If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>).</p><p>In the next lines there is a description of the teachers' matrix. Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> dominoes. The description of one domino is two integers (0 or 1), written without a space — the digits on the left and right half of the domino.</p>

## Output

<p>Print the resulting matrix of dominoes in the format: <span class="tex-span"><i>n</i></span> lines, each of them contains <span class="tex-span"><i>m</i></span> space-separated dominoes.</p><p>If there are multiple optimal solutions, print any of them.</p>





```input1
2 3
01 11 00
00 01 11

```




```input2
4 1
11
10
01
00

```




```output1
11 11 10
00 00 01

```




```output2
11
10
01
00

```



## Note

<p>Consider the answer for the first sample. There, the maximum sum among all columns equals <span class="tex-span">1</span> (the number of columns is <span class="tex-span">6</span>, and not <span class="tex-span">3</span>). Obviously, this maximum can't be less than <span class="tex-span">1</span>, then such matrix is optimal.</p><p>Note that the dominoes can be rotated by <span class="tex-span">180</span> degrees.</p>
