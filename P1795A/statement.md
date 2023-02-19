## Description

<div><p>There are two towers consisting of blocks of two colors: red and blue. Both towers are represented by strings of characters <span class="tex-font-style-tt">B</span> and/or <span class="tex-font-style-tt">R</span> denoting the order of blocks in them <span class="tex-font-style-bf">from the bottom to the top</span>, where <span class="tex-font-style-tt">B</span> corresponds to a blue block, and <span class="tex-font-style-tt">R</span> corresponds to a red block.</p><center> <img class="tex-graphics" src="file://8AHhtHnl.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">These two towers are represented by strings <span class="tex-font-style-tt">BRBB</span> and <span class="tex-font-style-tt">RBR</span>.</span> </center><p>You can perform the following operation any number of times: choose a tower with <span class="tex-font-style-bf">at least two blocks</span>, and move its <span class="tex-font-style-bf">top</span> block to the <span class="tex-font-style-bf">top</span> of the other tower.</p><center> <img class="tex-graphics" src="file://F1j9G2QQ.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://bVVXvDBR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The pair of towers is <span class="tex-font-style-it">beautiful</span> if no pair of touching blocks has the same color; i. e. no red block stands on top of another red block, and no blue block stands on top of another blue block.</p><p>You have to check if it is possible to perform any number of operations (possibly zero) to make the pair of towers beautiful.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of three lines:</p><ul> <li> the first line contains two integers $n$ and $m$ ($1 \le n, m \le 20$)&nbsp;— the number of blocks in the first tower and the number of blocks in the second tower, respectively; </li><li> the second line contains $s$&nbsp;— a string of exactly $n$ characters <span class="tex-font-style-tt">B</span> and/or <span class="tex-font-style-tt">R</span>, denoting the first tower; </li><li> the third line contains $t$&nbsp;— a string of exactly $m$ characters <span class="tex-font-style-tt">B</span> and/or <span class="tex-font-style-tt">R</span>, denoting the second tower. </li></ul></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to perform several (possibly zero) operations in such a way that the pair of towers becomes beautiful; otherwise print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of three lines:</p><ul> <li> the first line contains two integers $n$ and $m$ ($1 \le n, m \le 20$)&nbsp;— the number of blocks in the first tower and the number of blocks in the second tower, respectively; </li><li> the second line contains $s$&nbsp;— a string of exactly $n$ characters <span class="tex-font-style-tt">B</span> and/or <span class="tex-font-style-tt">R</span>, denoting the first tower; </li><li> the third line contains $t$&nbsp;— a string of exactly $m$ characters <span class="tex-font-style-tt">B</span> and/or <span class="tex-font-style-tt">R</span>, denoting the second tower. </li></ul>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to perform several (possibly zero) operations in such a way that the pair of towers becomes beautiful; otherwise print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p>





```input1|2,3,4,8,9,10
4
4 3
BRBB
RBR
4 7
BRBR
RRBRBRB
3 4
RBR
BRBR
5 4
BRBRR
BRBR
```




```output1
YES
YES
YES
NO
```



## Note

<p>In the first test case, you can move the top block from the first tower to the second tower (see the third picture).</p><p>In the second test case, you can move the top block from the second tower to the first tower $6$ times.</p><p>In the third test case, the pair of towers is already beautiful.</p>
