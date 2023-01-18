## Description

<div><p>You found a mysterious function <span class="tex-span"><i>f</i></span>. The function takes two strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. These strings must consist only of lowercase English letters, and must be the same length.</p><p>The output of the function <span class="tex-span"><i>f</i></span> is another string of the same length. The <span class="tex-span"><i>i</i></span>-th character of the output is equal to the minimum of the <span class="tex-span"><i>i</i></span>-th character of <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and the <span class="tex-span"><i>i</i></span>-th character of <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>.</p><p>For example, <span class="tex-span"><i>f</i>(</span>"<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>"<span class="tex-span">)</span> = "<span class="tex-font-style-tt">aa</span>", and <span class="tex-span"><i>f</i>(</span>"<span class="tex-font-style-tt">nzwzl</span>", "<span class="tex-font-style-tt">zizez</span>"<span class="tex-span">)</span> = "<span class="tex-font-style-tt">niwel</span>".</p><p>You found two strings <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> of the same length and consisting of only lowercase English letters. Find any string <span class="tex-span"><i>z</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>, <i>z</i>) = <i>y</i></span>, or print <span class="tex-font-style-tt">-1</span> if no such string <span class="tex-span"><i>z</i></span> exists.</p></div><div class="input-specification"><p>The first line of input contains the string <span class="tex-span"><i>x</i></span>.</p><p>The second line of input contains the string <span class="tex-span"><i>y</i></span>.</p><p>Both <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> consist only of lowercase English letters, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> have same length and this length is between <span class="tex-span">1</span> and <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>If there is no string <span class="tex-span"><i>z</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>, <i>z</i>) = <i>y</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print a string <span class="tex-span"><i>z</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>, <i>z</i>) = <i>y</i></span>. If there are multiple possible answers, print any of them. The string <span class="tex-span"><i>z</i></span> should be the same length as <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> and consist only of lowercase English letters.</p></div>

## Input

<p>The first line of input contains the string <span class="tex-span"><i>x</i></span>.</p><p>The second line of input contains the string <span class="tex-span"><i>y</i></span>.</p><p>Both <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> consist only of lowercase English letters, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> have same length and this length is between <span class="tex-span">1</span> and <span class="tex-span">100</span>.</p>

## Output

<p>If there is no string <span class="tex-span"><i>z</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>, <i>z</i>) = <i>y</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print a string <span class="tex-span"><i>z</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>, <i>z</i>) = <i>y</i></span>. If there are multiple possible answers, print any of them. The string <span class="tex-span"><i>z</i></span> should be the same length as <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> and consist only of lowercase English letters.</p>





```input1
ab
aa

```




```input2
nzwzl
niwel

```




```input3
ab
ba

```




```output1
ba

```




```output2
xiyez

```




```output3
-1

```



## Note

<p>The first case is from the statement.</p><p>Another solution for the second case is "<span class="tex-font-style-tt">zizez</span>"</p><p>There is no solution for the third case. That is, there is no <span class="tex-span"><i>z</i></span> such that <span class="tex-span"><i>f</i>(</span>"<span class="tex-font-style-tt">ab</span>", <span class="tex-span"><i>z</i>) = </span> "<span class="tex-font-style-tt">ba</span>".</p>
