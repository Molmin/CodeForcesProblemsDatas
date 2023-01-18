## Description

<div><p>You are given a matrix of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Each element of the matrix is either 1 or 0. You have to determine the number of connected components consisting of 1's. Two cells belong to the same component if they have a common border, and both elements in these cells are 1's.</p><p><span class="tex-font-style-bf">Note that the memory limit is unusual!</span></p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2<sup class="upper-index">12</sup></span>, <span class="tex-span">4 ≤ <i>m</i> ≤ 2<sup class="upper-index">14</sup></span>) — the number of rows and columns, respectively. It is guaranteed that <span class="tex-span"><i>m</i></span> is divisible by 4.</p><p>Then the representation of matrix follows. Each of <span class="tex-span"><i>n</i></span> next lines contains <img align="middle" class="tex-formula" src="file://IzqyFK95.png" style="max-width: 100.0%;max-height: 100.0%;"> one-digit hexadecimal numbers (that is, these numbers can be represented either as digits from <span class="tex-span">0</span> to <span class="tex-span">9</span> or as uppercase Latin letters from <span class="tex-span"><i>A</i></span> to <span class="tex-span"><i>F</i></span>). Binary representation of each of these numbers denotes next <span class="tex-span">4</span> elements of the matrix in the corresponding row. For example, if the number <span class="tex-span"><i>B</i></span> is given, then the corresponding elements are <span class="tex-font-style-tt">1011</span>, and if the number is <span class="tex-span">5</span>, then the corresponding elements are <span class="tex-font-style-tt">0101</span>.</p><p>Elements are not separated by whitespaces.</p></div><div class="output-specification"><p>Print the number of connected components consisting of 1's. </p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2<sup class="upper-index">12</sup></span>, <span class="tex-span">4 ≤ <i>m</i> ≤ 2<sup class="upper-index">14</sup></span>) — the number of rows and columns, respectively. It is guaranteed that <span class="tex-span"><i>m</i></span> is divisible by 4.</p><p>Then the representation of matrix follows. Each of <span class="tex-span"><i>n</i></span> next lines contains <img align="middle" class="tex-formula" src="file://IzqyFK95.png" style="max-width: 100.0%;max-height: 100.0%;"> one-digit hexadecimal numbers (that is, these numbers can be represented either as digits from <span class="tex-span">0</span> to <span class="tex-span">9</span> or as uppercase Latin letters from <span class="tex-span"><i>A</i></span> to <span class="tex-span"><i>F</i></span>). Binary representation of each of these numbers denotes next <span class="tex-span">4</span> elements of the matrix in the corresponding row. For example, if the number <span class="tex-span"><i>B</i></span> is given, then the corresponding elements are <span class="tex-font-style-tt">1011</span>, and if the number is <span class="tex-span">5</span>, then the corresponding elements are <span class="tex-font-style-tt">0101</span>.</p><p>Elements are not separated by whitespaces.</p>

## Output

<p>Print the number of connected components consisting of 1's. </p>





```input1
3 4
1
A
8

```




```input2
2 8
5F
E3

```




```input3
1 4
0

```




```output1
3

```




```output2
2

```




```output3
0

```



## Note

<p>In the first example the matrix is: </p><pre class="verbatim"><br>0001<br>1010<br>1000<br></pre><p>It is clear that it has three components.</p><p>The second example: </p><pre class="verbatim"><br>01011111<br>11100011<br></pre><p>It is clear that the number of components is 2.</p><p>There are no 1's in the third example, so the answer is 0.</p>
