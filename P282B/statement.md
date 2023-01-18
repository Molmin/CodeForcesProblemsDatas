## Description

<div><p>The Bitlandians are quite weird people. They have very peculiar customs.</p><p>As is customary, Uncle J. wants to have <span class="tex-span"><i>n</i></span> eggs painted for Bitruz (an ancient Bitland festival). He has asked G. and A. to do the work.</p><p>The kids are excited because just as is customary, they're going to be paid for the job! </p><p>Overall uncle J. has got <span class="tex-span"><i>n</i></span> eggs. G. named his price for painting each egg. Similarly, A. named his price for painting each egg. It turns out that for each egg the sum of the money both A. and G. want for the painting equals <span class="tex-span">1000</span>.</p><p>Uncle J. wants to distribute the eggs between the children so as to give each egg to exactly one child. Also, Uncle J. wants the total money paid to A. to be different from the total money paid to G. by no more than <span class="tex-span">500</span>.</p><p>Help Uncle J. Find the required distribution of eggs or otherwise say that distributing the eggs in the required manner is impossible.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of eggs.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> each <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 1000;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> + <i>g</i><sub class="lower-index"><i>i</i></sub> = 1000)</span>: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the price said by A. for the <span class="tex-span"><i>i</i></span>-th egg and <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> is the price said by G. for the <span class="tex-span"><i>i</i></span>-th egg.</p></div><div class="output-specification"><p>If it is impossible to assign the painting, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p><p>Otherwise print a string, consisting of <span class="tex-span"><i>n</i></span> letters "<span class="tex-font-style-tt">G</span>" and "<span class="tex-font-style-tt">A</span>". The <span class="tex-span"><i>i</i></span>-th letter of this string should represent the child who will get the <span class="tex-span"><i>i</i></span>-th egg in the required distribution. Letter "<span class="tex-font-style-tt">A</span>" represents A. and letter "<span class="tex-font-style-tt">G</span>" represents G. If we denote the money Uncle J. must pay A. for the painting as <span class="tex-span"><i>S</i><sub class="lower-index"><i>a</i></sub></span>, and the money Uncle J. must pay G. for the painting as <span class="tex-span"><i>S</i><sub class="lower-index"><i>g</i></sub></span>, then this inequality must hold: <span class="tex-span">|<i>S</i><sub class="lower-index"><i>a</i></sub>  -  <i>S</i><sub class="lower-index"><i>g</i></sub>|  ≤  500</span>. </p><p>If there are several solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of eggs.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> each <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 1000;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> + <i>g</i><sub class="lower-index"><i>i</i></sub> = 1000)</span>: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the price said by A. for the <span class="tex-span"><i>i</i></span>-th egg and <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> is the price said by G. for the <span class="tex-span"><i>i</i></span>-th egg.</p>

## Output

<p>If it is impossible to assign the painting, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p><p>Otherwise print a string, consisting of <span class="tex-span"><i>n</i></span> letters "<span class="tex-font-style-tt">G</span>" and "<span class="tex-font-style-tt">A</span>". The <span class="tex-span"><i>i</i></span>-th letter of this string should represent the child who will get the <span class="tex-span"><i>i</i></span>-th egg in the required distribution. Letter "<span class="tex-font-style-tt">A</span>" represents A. and letter "<span class="tex-font-style-tt">G</span>" represents G. If we denote the money Uncle J. must pay A. for the painting as <span class="tex-span"><i>S</i><sub class="lower-index"><i>a</i></sub></span>, and the money Uncle J. must pay G. for the painting as <span class="tex-span"><i>S</i><sub class="lower-index"><i>g</i></sub></span>, then this inequality must hold: <span class="tex-span">|<i>S</i><sub class="lower-index"><i>a</i></sub>  -  <i>S</i><sub class="lower-index"><i>g</i></sub>|  ≤  500</span>. </p><p>If there are several solutions, you are allowed to print any of them.</p>





```input1
2
1 999
999 1

```




```input2
3
400 600
400 600
400 600

```




```output1
AG

```




```output2
AGA

```


