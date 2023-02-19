## Description

<div><p>Artsem has a friend Saunders from University of Chicago. Saunders presented him with the following problem.</p><p>Let <span class="tex-span">[<i>n</i>]</span> denote the set <span class="tex-span">{1, ..., <i>n</i>}</span>. We will also write <span class="tex-span"><i>f</i>: [<i>x</i>] → [<i>y</i>]</span> when a function <span class="tex-span"><i>f</i></span> is defined in integer points <span class="tex-span">1</span>, ..., <span class="tex-span"><i>x</i></span>, and all its values are integers from 1 to <span class="tex-span"><i>y</i></span>.</p><p>Now then, you are given a function <span class="tex-span"><i>f</i>: [<i>n</i>] → [<i>n</i>]</span>. Your task is to find a positive integer <span class="tex-span"><i>m</i></span>, and two functions <span class="tex-span"><i>g</i>: [<i>n</i>] → [<i>m</i>]</span>, <span class="tex-span"><i>h</i>: [<i>m</i>] → [<i>n</i>]</span>, such that <span class="tex-span"><i>g</i>(<i>h</i>(<i>x</i>)) = <i>x</i></span> for all <img align="middle" class="tex-formula" src="file://b1PhhzBW.png" style="max-width: 100.0%;max-height: 100.0%;">, and <span class="tex-span"><i>h</i>(<i>g</i>(<i>x</i>)) = <i>f</i>(<i>x</i>)</span> for all <img align="middle" class="tex-formula" src="file://tKkhXoaf.png" style="max-width: 100.0%;max-height: 100.0%;">, or determine that finding these is impossible.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers&nbsp;— values <span class="tex-span"><i>f</i>(1), ..., <i>f</i>(<i>n</i>)</span> (<span class="tex-span">1 ≤ <i>f</i>(<i>i</i>) ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>If there is no answer, print one integer <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, on the first line print the number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>). On the second line print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>g</i>(1), ..., <i>g</i>(<i>n</i>)</span>. On the third line print <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>h</i>(1), ..., <i>h</i>(<i>m</i>)</span>.</p><p>If there are several correct answers, you may output any of them. It is guaranteed that if a valid answer exists, then there is an answer satisfying the above restrictions.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers&nbsp;— values <span class="tex-span"><i>f</i>(1), ..., <i>f</i>(<i>n</i>)</span> (<span class="tex-span">1 ≤ <i>f</i>(<i>i</i>) ≤ <i>n</i></span>).</p>

## Output

<p>If there is no answer, print one integer <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, on the first line print the number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>). On the second line print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>g</i>(1), ..., <i>g</i>(<i>n</i>)</span>. On the third line print <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>h</i>(1), ..., <i>h</i>(<i>m</i>)</span>.</p><p>If there are several correct answers, you may output any of them. It is guaranteed that if a valid answer exists, then there is an answer satisfying the above restrictions.</p>





```input1
3
1 2 3

```




```input2
3
2 2 2

```




```input3
2
2 1

```




```output1
3
1 2 3
1 2 3

```




```output2
1
1 1 1
2

```




```output3
-1

```


