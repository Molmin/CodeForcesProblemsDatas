## Description

<div><p>An <span class="tex-span"><i>n</i> × <i>n</i></span> square matrix is <span class="tex-font-style-it">special</span>, if:</p><ul> <li> it is binary, that is, each cell contains either a 0, or a 1; </li><li> the number of ones in each row and column equals 2. </li></ul><p>You are given <span class="tex-span"><i>n</i></span> and the first <span class="tex-span"><i>m</i></span> rows of the matrix. Print the number of special <span class="tex-span"><i>n</i> × <i>n</i></span> matrices, such that the first <span class="tex-span"><i>m</i></span> rows coincide with the given ones.</p><p>As the required value can be rather large, print the remainder after dividing the value by the given number <span class="tex-span"><i>mod</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">2 ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup></span>). Then <span class="tex-span"><i>m</i></span> lines follow, each of them contains <span class="tex-span"><i>n</i></span> characters — the first rows of the required special matrices. Each of these lines contains exactly two characters '<span class="tex-font-style-tt">1</span>', the rest characters are '<span class="tex-font-style-tt">0</span>'. Each column of the given <span class="tex-span"><i>m</i> × <i>n</i></span> table contains at most two numbers one.</p></div><div class="output-specification"><p>Print the remainder after dividing the required value by number <span class="tex-span"><i>mod</i></span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">2 ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup></span>). Then <span class="tex-span"><i>m</i></span> lines follow, each of them contains <span class="tex-span"><i>n</i></span> characters — the first rows of the required special matrices. Each of these lines contains exactly two characters '<span class="tex-font-style-tt">1</span>', the rest characters are '<span class="tex-font-style-tt">0</span>'. Each column of the given <span class="tex-span"><i>m</i> × <i>n</i></span> table contains at most two numbers one.</p>

## Output

<p>Print the remainder after dividing the required value by number <span class="tex-span"><i>mod</i></span>.</p>





```input1
3 1 1000
011

```




```input2
4 4 100500
0110
1010
0101
1001

```




```output1
2

```




```output2
1

```



## Note

<p>For the first test the required matrices are: </p><pre class="verbatim"><br>011<br>101<br>110<br><br>011<br>110<br>101<br></pre><p>In the second test the required matrix is already fully given, so the answer is 1.</p>
