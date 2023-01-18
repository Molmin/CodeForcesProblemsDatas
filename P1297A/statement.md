## Description

<div><p>Polycarp is working on the implementation of displaying likes on the Codehorses social network. The number of likes should be displayed in a format that will be easy to read by users. It was decided that for large numbers of likes the format should be like <span class="tex-font-style-tt">123K</span> (one hundred twenty-three thousand) or like <span class="tex-font-style-tt">56M</span> (fifty-six million).</p><p>The following displaying strategy has been approved:</p><ul> <li> the number will be displayed either as an integer number from <span class="tex-font-style-tt">0</span> to <span class="tex-font-style-tt">999</span>, or as a positive integer number of thousands (from <span class="tex-font-style-tt">1K</span> to <span class="tex-font-style-tt">999K</span>), or as a positive integer number of millions (from <span class="tex-font-style-tt">1M</span> on), </li><li> the specified exact number of likes $n$ when displaying should be rounded to the nearest view from the case above (if rounding is ambiguous, it must be rounded up): for example, $1785$ should be rounded to <span class="tex-font-style-tt">2K</span> instead of <span class="tex-font-style-tt">1K</span>, $4500000$ should be rounded to <span class="tex-font-style-tt">5M</span>. </li></ul><p>Help Polycarp implement this part of the functionality: for a given non-negative integer number of likes $n$, print its view in the Codehorses interface.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$) — the number of test cases in the input. The following are descriptions of the $t$ input test cases, one per line.</p><p>The description of each test case consists of a single line that contains a non-negative integer $n$ ($0 \le n \le 2\cdot10^9$) — the number of likes.</p></div><div class="output-specification"><p>Print $t$ answers to the given test cases in the order from the input. Each printed value must have one of the following types:</p><ul> <li> either an integer from <span class="tex-font-style-tt">0</span> to <span class="tex-font-style-tt">999</span> which corresponds just to the number of likes, </li><li> or a number of thousands from <span class="tex-font-style-tt">1K</span> to <span class="tex-font-style-tt">999K</span>, </li><li> or a number of millions from <span class="tex-font-style-tt">1M</span> to <span class="tex-font-style-tt">2000M</span>. </li></ul><p>The answer is equal to a view which is the closest (by difference) to the given number $n$. If this rounding is ambiguous, then round answer up (to a greater value).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$) — the number of test cases in the input. The following are descriptions of the $t$ input test cases, one per line.</p><p>The description of each test case consists of a single line that contains a non-negative integer $n$ ($0 \le n \le 2\cdot10^9$) — the number of likes.</p>

## Output

<p>Print $t$ answers to the given test cases in the order from the input. Each printed value must have one of the following types:</p><ul> <li> either an integer from <span class="tex-font-style-tt">0</span> to <span class="tex-font-style-tt">999</span> which corresponds just to the number of likes, </li><li> or a number of thousands from <span class="tex-font-style-tt">1K</span> to <span class="tex-font-style-tt">999K</span>, </li><li> or a number of millions from <span class="tex-font-style-tt">1M</span> to <span class="tex-font-style-tt">2000M</span>. </li></ul><p>The answer is equal to a view which is the closest (by difference) to the given number $n$. If this rounding is ambiguous, then round answer up (to a greater value).</p>





```input1
9
999
123
0
1782
31415926
1500
999999
35499710
2000000000
```




```output1
999
123
0
2K
31M
2K
1M
35M
2000M
```



## Note

<p>Let's describe some test cases: </p><ul> <li> $1782$ can be displayed either as <span class="tex-font-style-tt">1K</span> or as <span class="tex-font-style-tt">2K</span> but <span class="tex-font-style-tt">2K</span> is the nearest view; </li><li> $1500$ have same difference with <span class="tex-font-style-tt">1K</span> and <span class="tex-font-style-tt">2K</span> so it should be rounded up; </li><li> $999999$ should be displayed as <span class="tex-font-style-tt">1M</span> since it's closer to it than to <span class="tex-font-style-tt">999K</span>. </li></ul>
