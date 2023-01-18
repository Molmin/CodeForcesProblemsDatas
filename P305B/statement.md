## Description

<div><p>A continued fraction of height <span class="tex-span"><i>n</i></span> is a fraction of form <img align="middle" class="tex-formula" src="file://0MJVv5nU.png" style="max-width: 100.0%;max-height: 100.0%;">. You are given two rational numbers, one is represented as <img align="middle" class="tex-formula" src="file://yoAIjOM0.png" style="max-width: 100.0%;max-height: 100.0%;"> and the other one is represented as a finite fraction of height <span class="tex-span"><i>n</i></span>. Check if they are equal.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>p</i>, <i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ <i>p</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the numerator and the denominator of the first fraction.</p><p>The second line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 90)</span> — the height of the second fraction. The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup>)</span> — the continued fraction.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if these fractions are equal and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>p</i>, <i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ <i>p</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the numerator and the denominator of the first fraction.</p><p>The second line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 90)</span> — the height of the second fraction. The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup>)</span> — the continued fraction.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if these fractions are equal and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
9 4
2
2 4

```




```input2
9 4
3
2 3 1

```




```input3
9 4
3
1 2 4

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first sample <img align="middle" class="tex-formula" src="file://WPr8yYhh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample <img align="middle" class="tex-formula" src="file://1vzDM2JR.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third sample <img align="middle" class="tex-formula" src="file://LXx4simt.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
