## Description

<div><p>You are given a matrix <span class="tex-span"><i>f</i></span> with <span class="tex-span">4</span> rows and <span class="tex-span"><i>n</i></span> columns. Each element of the matrix is either an asterisk (<span class="tex-font-style-tt">*</span>) or a dot (<span class="tex-font-style-tt">.</span>).</p><p>You may perform the following operation arbitrary number of times: choose a square submatrix of <span class="tex-span"><i>f</i></span> with size <span class="tex-span"><i>k</i> × <i>k</i></span> (where <span class="tex-span">1 ≤ <i>k</i> ≤ 4</span>) and replace each element of the chosen submatrix with a dot. Choosing a submatrix of size <span class="tex-span"><i>k</i> × <i>k</i></span> costs <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> coins.</p><p>What is the minimum number of coins you have to pay to replace all asterisks with dots?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>) — the number of columns in <span class="tex-span"><i>f</i></span>.</p><p>The second line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the cost to replace the square submatrix of size <span class="tex-span">1 × 1</span>, <span class="tex-span">2 × 2</span>, <span class="tex-span">3 × 3</span> or <span class="tex-span">4 × 4</span>, respectively.</p><p>Then four lines follow, each containing <span class="tex-span"><i>n</i></span> characters and denoting a row of matrix <span class="tex-span"><i>f</i></span>. Each character is either a dot or an asterisk.</p></div><div class="output-specification"><p>Print one integer — the minimum number of coins to replace all asterisks with dots.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>) — the number of columns in <span class="tex-span"><i>f</i></span>.</p><p>The second line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the cost to replace the square submatrix of size <span class="tex-span">1 × 1</span>, <span class="tex-span">2 × 2</span>, <span class="tex-span">3 × 3</span> or <span class="tex-span">4 × 4</span>, respectively.</p><p>Then four lines follow, each containing <span class="tex-span"><i>n</i></span> characters and denoting a row of matrix <span class="tex-span"><i>f</i></span>. Each character is either a dot or an asterisk.</p>

## Output

<p>Print one integer — the minimum number of coins to replace all asterisks with dots.</p>





```input1
4
1 10 8 20
***.
***.
***.
...*

```




```input2
7
2 1 8 2
.***...
.***..*
.***...
....*..

```




```input3
4
10 10 1 10
***.
*..*
*..*
.***

```




```output1
9

```




```output2
3

```




```output3
2

```



## Note

<p>In the first example you can spend <span class="tex-span">8</span> coins to replace the submatrix <span class="tex-span">3 × 3</span> in the top-left corner, and <span class="tex-span">1</span> coin to replace the <span class="tex-span">1 × 1</span> submatrix in the bottom-right corner.</p><p>In the second example the best option is to replace the <span class="tex-span">4 × 4</span> submatrix containing columns <span class="tex-span">2 – 5</span>, and the <span class="tex-span">2 × 2</span> submatrix consisting of rows <span class="tex-span">2 – 3</span> and columns <span class="tex-span">6 – 7</span>.</p><p>In the third example you can select submatrix <span class="tex-span">3 × 3</span> in the top-left corner and then submatrix <span class="tex-span">3 × 3</span> consisting of rows <span class="tex-span">2 – 4</span> and columns <span class="tex-span">2 – 4</span>.</p>
