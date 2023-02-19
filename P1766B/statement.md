## Description

<div><p>You want to type the string $s$, consisting of $n$ lowercase Latin letters, using your favorite text editor Notepad#.</p><p>Notepad# supports two kinds of operations: </p><ul> <li> append any letter <span class="tex-font-style-bf">to the end</span> of the string; </li><li> copy a <span class="tex-font-style-bf">continuous</span> substring of an already typed string and paste this substring <span class="tex-font-style-bf">to the end</span> of the string. </li></ul><p>Can you type string $s$ in <span class="tex-font-style-bf">strictly less</span> than $n$ operations?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string $s$.</p><p>The second line contains a string $s$, consisting of $n$ lowercase Latin letters.</p><p>The sum of $n$ doesn't exceed $2 \cdot 10^5$ over all testcases.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if you can type string $s$ in <span class="tex-font-style-bf">strictly less</span> than $n$ operations. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string $s$.</p><p>The second line contains a string $s$, consisting of $n$ lowercase Latin letters.</p><p>The sum of $n$ doesn't exceed $2 \cdot 10^5$ over all testcases.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if you can type string $s$ in <span class="tex-font-style-bf">strictly less</span> than $n$ operations. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|2,3,6,7,10,11
6
10
codeforces
8
labacaba
5
uohhh
16
isthissuffixtree
1
x
4
momo
```




```output1
NO
YES
NO
YES
NO
YES
```



## Note

<p>In the first testcase, you can start with typing "<span class="tex-font-style-tt">codef</span>" ($5$ operations), then copy "<span class="tex-font-style-tt">o</span>" ($1$ operation) from an already typed part, then finish with typing "<span class="tex-font-style-tt">rces</span>" ($4$ operations). That will be $10$ operations, which is not strictly less than $n$. There exist other ways to type "<span class="tex-font-style-tt">codeforces</span>". However, no matter what you do, you can't do less than $n$ operations.</p><p>In the second testcase, you can type "<span class="tex-font-style-tt">labac</span>" ($5$ operations), then copy "<span class="tex-font-style-tt">aba</span>" ($1$ operation), finishing the string in $6$ operations.</p>
