## Description

<div><p>A chocolate bar has a rectangular shape and consists of <span class="tex-span"><i>n</i> × <i>m</i></span> slices. In other words, a bar consists of <span class="tex-span"><i>n</i></span> rows with <span class="tex-span"><i>m</i></span> slices of chocolate in each row.</p><p>Each slice of chocolate is known to weigh 1 gram. Your task is to determine for each of the <span class="tex-span"><i>q</i></span> chocolate bars whether it is possible to obtain a piece weighing <span class="tex-span"><i>p</i></span> grams by breaking the bar several (possibly zero) times. The final piece of the chocolate bar should be whole, and breaks are made along the line of slices' section for the whole length of the current piece.</p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100</span>) — the number of chocolate bars. </p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>p</i> ≤ 1000</span>) — the size of the chocolate bar, and the weight of the piece which should be obtained.</p></div><div class="output-specification"><p>The output should contain <span class="tex-span"><i>q</i></span> lines and the <span class="tex-span"><i>i</i></span>-th line must contain "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if it is possible to perform the task for <span class="tex-span"><i>i</i></span>-th chocolate bar, or "<span class="tex-font-style-tt">No</span>" otherwise.</p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100</span>) — the number of chocolate bars. </p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>p</i> ≤ 1000</span>) — the size of the chocolate bar, and the weight of the piece which should be obtained.</p>

## Output

<p>The output should contain <span class="tex-span"><i>q</i></span> lines and the <span class="tex-span"><i>i</i></span>-th line must contain "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if it is possible to perform the task for <span class="tex-span"><i>i</i></span>-th chocolate bar, or "<span class="tex-font-style-tt">No</span>" otherwise.</p>





```input1
2
3 3 4
4 4 7

```




```output1
Yes
No

```


