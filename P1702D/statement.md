## Description

<div><p>Let $s$ be a string of lowercase Latin letters. Its price is the sum of the indices of letters (an integer between 1 and 26) that are included in it. For example, the price of the string <span class="tex-font-style-tt">abca</span> is $1+2+3+1=7$.</p><p>The string $w$ and the integer $p$ are given. Remove the minimal number of letters from $w$ so that its price becomes less than or equal to $p$ and print the resulting string. Note that the resulting string may be empty. You can delete arbitrary letters, they do not have to go in a row. If the price of a given string $w$ is less than or equal to $p$, then nothing needs to be deleted and $w$ must be output.</p><p>Note that when you delete a letter from $w$, the order of the remaining letters is preserved. For example, if you delete the letter <span class="tex-font-style-tt">e</span> from the string <span class="tex-font-style-tt">test</span>, you get <span class="tex-font-style-tt">tst</span>.</p></div><div class="input-specification"><p>The first line of input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test. The following are descriptions of $t$ test cases.</p><p>Each case consists of two lines.</p><p>The first of them is the string $w$, it is non-empty and consists of lowercase Latin letters. Its length does not exceed $2\cdot10^5$.</p><p>The second line contains an integer $p$ ($1 \le p \le 5\,200\,000$).</p><p>It is guaranteed that the sum of string lengths $w$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output exactly $t$ rows, the $i$-th of them should contain the answer to the $i$-th set of input data. Print the longest string that is obtained from $w$ by deleting letters such that its price is less or equal to $p$. If there are several answers, then output any of them.</p><p>Note that the empty string &nbsp;— is one of the possible answers. In this case, just output an empty string.</p></div>

## Input

<p>The first line of input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the test. The following are descriptions of $t$ test cases.</p><p>Each case consists of two lines.</p><p>The first of them is the string $w$, it is non-empty and consists of lowercase Latin letters. Its length does not exceed $2\cdot10^5$.</p><p>The second line contains an integer $p$ ($1 \le p \le 5\,200\,000$).</p><p>It is guaranteed that the sum of string lengths $w$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output exactly $t$ rows, the $i$-th of them should contain the answer to the $i$-th set of input data. Print the longest string that is obtained from $w$ by deleting letters such that its price is less or equal to $p$. If there are several answers, then output any of them.</p><p>Note that the empty string &nbsp;— is one of the possible answers. In this case, just output an empty string.</p>





```input1|2,3,6,7,10,11
5
abca
2
abca
6
codeforces
1
codeforces
10
codeforces
100
```




```output1
aa
abc

cdc
codeforces
```


