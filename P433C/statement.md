## Description

<div><p>Ryouko is an extremely forgetful girl, she could even forget something that has just happened. So in order to remember, she takes a notebook with her, called <span class="tex-font-style-it">Ryouko's Memory Note</span>. She writes what she sees and what she hears on the notebook, and the notebook became her memory.</p><p>Though Ryouko is forgetful, she is also born with superb analyzing abilities. However, analyzing depends greatly on gathered information, in other words, memory. So she has to shuffle through her notebook whenever she needs to analyze, which is tough work.</p><p>Ryouko's notebook consists of <span class="tex-span"><i>n</i></span> pages, numbered from 1 to <span class="tex-span"><i>n</i></span>. To make life (and this problem) easier, we consider that to turn from page <span class="tex-span"><i>x</i></span> to page <span class="tex-span"><i>y</i></span>, <span class="tex-span">|<i>x</i> - <i>y</i>|</span> pages should be turned. During analyzing, Ryouko needs <span class="tex-span"><i>m</i></span> pieces of information, the <span class="tex-span"><i>i</i></span>-th piece of information is on page <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Information must be read from the notebook in order, so the total number of pages that Ryouko needs to turn is <img align="middle" class="tex-formula" src="file://qTrZZDan.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Ryouko wants to decrease the number of pages that need to be turned. In order to achieve this, she can merge two pages of her notebook. If Ryouko merges page <span class="tex-span"><i>x</i></span> to page <span class="tex-span"><i>y</i></span>, she would copy all the information on page <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i>&nbsp;(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span>, and consequently, all elements in sequence <span class="tex-span"><i>a</i></span> that was <span class="tex-span"><i>x</i></span> would become <span class="tex-span"><i>y</i></span>. Note that <span class="tex-span"><i>x</i></span> can be equal to <span class="tex-span"><i>y</i></span>, in which case no changes take place.</p><p>Please tell Ryouko the minimum number of pages that she needs to turn. Note she can apply the described operation at most once before the reading. Note that the answer can exceed 32-bit integers.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next line contains <span class="tex-span"><i>m</i></span> integers separated by spaces: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of pages Ryouko needs to turn.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next line contains <span class="tex-span"><i>m</i></span> integers separated by spaces: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print a single integer — the minimum number of pages Ryouko needs to turn.</p>





```input1
4 6
1 2 3 4 3 2

```




```input2
10 5
9 4 3 8 8

```




```output1
3

```




```output2
6

```



## Note

<p>In the first sample, the optimal solution is to merge page 4 to 3, after merging sequence <span class="tex-span"><i>a</i></span> becomes <span class="tex-span">{1, 2, 3, 3, 3, 2}</span>, so the number of pages Ryouko needs to turn is <span class="tex-span">|1 - 2| + |2 - 3| + |3 - 3| + |3 - 3| + |3 - 2| = 3</span>.</p><p>In the second sample, optimal solution is achieved by merging page 9 to 4.</p>
