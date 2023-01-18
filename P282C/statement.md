## Description

<div><p>The Bitlandians are quite weird people. They do everything differently. They have a different alphabet so they have a different definition for a string.</p><p>A Bitlandish string is a string made only of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>".</p><p>BitHaval (the mayor of Bitland) loves to play with Bitlandish strings. He takes some Bitlandish string <span class="tex-span"><i>a</i></span>, and applies several (possibly zero) operations to it. In one operation the mayor may take any two adjacent characters of a string, define one of them as <span class="tex-span"><i>x</i></span> and the other one as <span class="tex-span"><i>y</i></span>. Then he calculates two values <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>: <span class="tex-span"><i>p</i> = <i>x</i>&nbsp;<i>xor</i>&nbsp;<i>y</i></span>, <span class="tex-span"><i>q</i> = <i>x</i>&nbsp;<i>or</i>&nbsp;<i>y</i></span>. Then he replaces one of the two taken characters by <span class="tex-span"><i>p</i></span> and the other one by <span class="tex-span"><i>q</i></span>.</p><p>The <span class="tex-span"><i>xor</i></span> operation means the bitwise excluding OR operation. The <span class="tex-span"><i>or</i></span> operation is the bitwise OR operation.</p><p>So for example one operation can transform string <span class="tex-font-style-tt">11</span> to string <span class="tex-font-style-tt">10</span> or to string <span class="tex-font-style-tt">01</span>. String <span class="tex-font-style-tt">1</span> cannot be transformed into any other string.</p><p>You've got two Bitlandish strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Your task is to check if it is possible for BitHaval to transform string <span class="tex-span"><i>a</i></span> to string <span class="tex-span"><i>b</i></span> in several (possibly zero) described operations.</p></div><div class="input-specification"><p>The first line contains Bitlandish string <span class="tex-span"><i>a</i></span>, the second line contains Bitlandish string <span class="tex-span"><i>b</i></span>. The strings can have different lengths.</p><p>It is guaranteed that the given strings only consist of characters "0" and "1". The strings are not empty, their length doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if <span class="tex-span"><i>a</i></span> can be transformed into <span class="tex-span"><i>b</i></span>, otherwise print "<span class="tex-font-style-tt">NO</span>". Please do not print the quotes.</p></div>

## Input

<p>The first line contains Bitlandish string <span class="tex-span"><i>a</i></span>, the second line contains Bitlandish string <span class="tex-span"><i>b</i></span>. The strings can have different lengths.</p><p>It is guaranteed that the given strings only consist of characters "0" and "1". The strings are not empty, their length doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if <span class="tex-span"><i>a</i></span> can be transformed into <span class="tex-span"><i>b</i></span>, otherwise print "<span class="tex-font-style-tt">NO</span>". Please do not print the quotes.</p>





```input1
11
10

```




```input2
1
01

```




```input3
000
101

```




```output1
YES

```




```output2
NO

```




```output3
NO

```


