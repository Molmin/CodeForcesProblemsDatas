## Description

<div><p>Some time ago Leonid have known about <span class="tex-font-style-it">idempotent functions</span>. <span class="tex-font-style-it">Idempotent function</span> defined on a set <span class="tex-span">{1, 2, ..., <i>n</i>}</span> is such function <img align="middle" class="tex-formula" src="file://iDE04sTB.png" style="max-width: 100.0%;max-height: 100.0%;">, that for any <img align="middle" class="tex-formula" src="file://LLECBPPc.png" style="max-width: 100.0%;max-height: 100.0%;"> the formula <span class="tex-span"><i>g</i>(<i>g</i>(<i>x</i>)) = <i>g</i>(<i>x</i>)</span> holds.</p><p>Let's denote as <span class="tex-span"><i>f</i><sup class="upper-index">(<i>k</i>)</sup>(<i>x</i>)</span> the function <span class="tex-span"><i>f</i></span> applied <span class="tex-span"><i>k</i></span> times to the value <span class="tex-span"><i>x</i></span>. More formally, <span class="tex-span"><i>f</i><sup class="upper-index">(1)</sup>(<i>x</i>) = <i>f</i>(<i>x</i>)</span>, <span class="tex-span"><i>f</i><sup class="upper-index">(<i>k</i>)</sup>(<i>x</i>) = <i>f</i>(<i>f</i><sup class="upper-index">(<i>k</i> - 1)</sup>(<i>x</i>))</span> for each <span class="tex-span"><i>k</i> &gt; 1</span>.</p><p>You are given some function <img align="middle" class="tex-formula" src="file://bvlhOxrX.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to find minimum positive integer <span class="tex-span"><i>k</i></span> such that function <span class="tex-span"><i>f</i><sup class="upper-index">(<i>k</i>)</sup>(<i>x</i>)</span> is <span class="tex-font-style-it">idempotent</span>.</p></div><div class="input-specification"><p>In the first line of the input there is a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the size of function <span class="tex-span"><i>f</i></span> domain.</p><p>In the second line follow <span class="tex-span"><i>f</i>(1), <i>f</i>(2), ..., <i>f</i>(<i>n</i>)</span> (<span class="tex-span">1 ≤ <i>f</i>(<i>i</i>) ≤ <i>n</i></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), the values of a function.</p></div><div class="output-specification"><p>Output minimum <span class="tex-span"><i>k</i></span> such that function <span class="tex-span"><i>f</i><sup class="upper-index">(<i>k</i>)</sup>(<i>x</i>)</span> is <span class="tex-font-style-it">idempotent</span>.</p></div>

## Input

<p>In the first line of the input there is a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the size of function <span class="tex-span"><i>f</i></span> domain.</p><p>In the second line follow <span class="tex-span"><i>f</i>(1), <i>f</i>(2), ..., <i>f</i>(<i>n</i>)</span> (<span class="tex-span">1 ≤ <i>f</i>(<i>i</i>) ≤ <i>n</i></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), the values of a function.</p>

## Output

<p>Output minimum <span class="tex-span"><i>k</i></span> such that function <span class="tex-span"><i>f</i><sup class="upper-index">(<i>k</i>)</sup>(<i>x</i>)</span> is <span class="tex-font-style-it">idempotent</span>.</p>





```input1
4
1 2 2 4

```




```input2
3
2 3 3

```




```input3
3
2 3 1

```




```output1
1

```




```output2
2

```




```output3
3

```



## Note

<p>In the first sample test function <span class="tex-span"><i>f</i>(<i>x</i>) = <i>f</i><sup class="upper-index">(1)</sup>(<i>x</i>)</span> is already idempotent since <span class="tex-span"><i>f</i>(<i>f</i>(1)) = <i>f</i>(1) = 1</span>, <span class="tex-span"><i>f</i>(<i>f</i>(2)) = <i>f</i>(2) = 2</span>, <span class="tex-span"><i>f</i>(<i>f</i>(3)) = <i>f</i>(3) = 2</span>, <span class="tex-span"><i>f</i>(<i>f</i>(4)) = <i>f</i>(4) = 4</span>.</p><p>In the second sample test: </p><ul> <li> function <span class="tex-span"><i>f</i>(<i>x</i>) = <i>f</i><sup class="upper-index">(1)</sup>(<i>x</i>)</span> isn't idempotent because <span class="tex-span"><i>f</i>(<i>f</i>(1)) = 3</span> but <span class="tex-span"><i>f</i>(1) = 2</span>; </li><li> function <span class="tex-span"><i>f</i>(<i>x</i>) = <i>f</i><sup class="upper-index">(2)</sup>(<i>x</i>)</span> is idempotent since for any <span class="tex-span"><i>x</i></span> it is true that <span class="tex-span"><i>f</i><sup class="upper-index">(2)</sup>(<i>x</i>) = 3</span>, so it is also true that <span class="tex-span"><i>f</i><sup class="upper-index">(2)</sup>(<i>f</i><sup class="upper-index">(2)</sup>(<i>x</i>)) = 3</span>. </li></ul><p>In the third sample test: </p><ul> <li> function <span class="tex-span"><i>f</i>(<i>x</i>) = <i>f</i><sup class="upper-index">(1)</sup>(<i>x</i>)</span> isn't idempotent because <span class="tex-span"><i>f</i>(<i>f</i>(1)) = 3</span> but <span class="tex-span"><i>f</i>(1) = 2</span>; </li><li> function <span class="tex-span"><i>f</i>(<i>f</i>(<i>x</i>)) = <i>f</i><sup class="upper-index">(2)</sup>(<i>x</i>)</span> isn't idempotent because <span class="tex-span"><i>f</i><sup class="upper-index">(2)</sup>(<i>f</i><sup class="upper-index">(2)</sup>(1)) = 2</span> but <span class="tex-span"><i>f</i><sup class="upper-index">(2)</sup>(1) = 3</span>; </li><li> function <span class="tex-span"><i>f</i>(<i>f</i>(<i>f</i>(<i>x</i>))) = <i>f</i><sup class="upper-index">(3)</sup>(<i>x</i>)</span> is idempotent since it is identity function: <span class="tex-span"><i>f</i><sup class="upper-index">(3)</sup>(<i>x</i>) = <i>x</i></span> for any <img align="middle" class="tex-formula" src="file://QcZ1uHWa.png" style="max-width: 100.0%;max-height: 100.0%;"> meaning that the formula <span class="tex-span"><i>f</i><sup class="upper-index">(3)</sup>(<i>f</i><sup class="upper-index">(3)</sup>(<i>x</i>)) = <i>f</i><sup class="upper-index">(3)</sup>(<i>x</i>)</span> also holds. </li></ul>
