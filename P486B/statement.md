## Description

<div><p>Let's define logical <span class="tex-span"><i>OR</i></span> as an operation on two logical values (i. e. values that belong to the set <span class="tex-span">{0, 1}</span>) that is equal to <span class="tex-span">1</span> if either or both of the logical values is set to <span class="tex-span">1</span>, otherwise it is <span class="tex-span">0</span>. We can define logical <span class="tex-span"><i>OR</i></span> of three or more logical values in the same manner:</p><p><img align="middle" class="tex-formula" src="file://lwOUdfQp.png" style="max-width: 100.0%;max-height: 100.0%;"> where <img align="middle" class="tex-formula" src="file://TRJ96CPc.png" style="max-width: 100.0%;max-height: 100.0%;"> is equal to <span class="tex-span">1</span> if some <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span>, otherwise it is equal to <span class="tex-span">0</span>.</p><p>Nam has a matrix <span class="tex-span"><i>A</i></span> consisting of <span class="tex-span"><i>m</i></span> rows and <span class="tex-span"><i>n</i></span> columns. The rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Element at row <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) and column <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) is denoted as <span class="tex-span"><i>A</i><sub class="lower-index"><i>ij</i></sub></span>. All elements of <span class="tex-span"><i>A</i></span> are either 0 or 1. From matrix <span class="tex-span"><i>A</i></span>, Nam creates another matrix <span class="tex-span"><i>B</i></span> of the same size using formula:</p><p><img align="middle" class="tex-formula" src="file://jWqkguo7.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>(<span class="tex-span"><i>B</i><sub class="lower-index"><i>ij</i></sub></span> is <span class="tex-span"><i>OR</i></span> of all elements in row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span> of matrix <span class="tex-span"><i>A</i></span>)</p><p>Nam gives you matrix <span class="tex-span"><i>B</i></span> and challenges you to guess matrix <span class="tex-span"><i>A</i></span>. Although Nam is smart, he could probably make a mistake while calculating matrix <span class="tex-span"><i>B</i></span>, since size of <span class="tex-span"><i>A</i></span> can be large.</p></div><div class="input-specification"><p>The first line contains two integer <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 100</span>), number of rows and number of columns of matrices respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines each contain <span class="tex-span"><i>n</i></span> integers separated by spaces describing rows of matrix <span class="tex-span"><i>B</i></span> (each element of <span class="tex-span"><i>B</i></span> is either <span class="tex-span">0</span> or <span class="tex-span">1</span>).</p></div><div class="output-specification"><p>In the first line, print "<span class="tex-font-style-tt">NO</span>" if Nam has made a mistake when calculating <span class="tex-span"><i>B</i></span>, otherwise print "<span class="tex-font-style-tt">YES</span>". If the first line is "<span class="tex-font-style-tt">YES</span>", then also print <span class="tex-span"><i>m</i></span> rows consisting of <span class="tex-span"><i>n</i></span> integers representing matrix <span class="tex-span"><i>A</i></span> that can produce given matrix <span class="tex-span"><i>B</i></span>. If there are several solutions print any one.</p></div>

## Input

<p>The first line contains two integer <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>n</i> ≤ 100</span>), number of rows and number of columns of matrices respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines each contain <span class="tex-span"><i>n</i></span> integers separated by spaces describing rows of matrix <span class="tex-span"><i>B</i></span> (each element of <span class="tex-span"><i>B</i></span> is either <span class="tex-span">0</span> or <span class="tex-span">1</span>).</p>

## Output

<p>In the first line, print "<span class="tex-font-style-tt">NO</span>" if Nam has made a mistake when calculating <span class="tex-span"><i>B</i></span>, otherwise print "<span class="tex-font-style-tt">YES</span>". If the first line is "<span class="tex-font-style-tt">YES</span>", then also print <span class="tex-span"><i>m</i></span> rows consisting of <span class="tex-span"><i>n</i></span> integers representing matrix <span class="tex-span"><i>A</i></span> that can produce given matrix <span class="tex-span"><i>B</i></span>. If there are several solutions print any one.</p>





```input1
2 2
1 0
0 0

```




```input2
2 3
1 1 1
1 1 1

```




```input3
2 3
0 1 0
1 1 1

```




```output1
NO

```




```output2
YES
1 1 1
1 1 1

```




```output3
YES
0 0 0
0 1 0

```


