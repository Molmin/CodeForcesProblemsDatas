## Description

<div><p>String can be called <span class="tex-font-style-it">correct</span> if it consists of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>" and there are no redundant leading zeroes. Here are some examples: "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">1001</span>".</p><p>You are given a <span class="tex-font-style-it">correct</span> string <span class="tex-span"><i>s</i></span>.</p><p>You can perform two different operations on this string: </p><ol> <li> swap any pair of adjacent characters (for example, "<span class="tex-font-style-tt">1<span class="tex-font-style-underline">01</span></span>" <img align="middle" class="tex-formula" src="file://TAjBUzbc.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">1<span class="tex-font-style-underline">10</span></span>"); </li><li> replace "<span class="tex-font-style-tt">11</span>" with "<span class="tex-font-style-tt">1</span>" (for example, "<span class="tex-font-style-tt"><span class="tex-font-style-underline">11</span>0</span>" <img align="middle" class="tex-formula" src="file://lQ1WUx1n.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt"><span class="tex-font-style-underline">1</span>0</span>"). </li></ol><p>Let <span class="tex-span"><i>val</i>(<i>s</i>)</span> be such a number that <span class="tex-span"><i>s</i></span> is its binary representation.</p><p><span class="tex-font-style-it">Correct</span> string <span class="tex-span"><i>a</i></span> is less than some other <span class="tex-font-style-it">correct</span> string <span class="tex-span"><i>b</i></span> iff <span class="tex-span"><i>val</i>(<i>a</i>) &lt; <i>val</i>(<i>b</i>)</span>.</p><p>Your task is to find the minimum <span class="tex-font-style-it">correct</span> string that you can obtain from the given one using the operations described above. You can use these operations any number of times in any order (or even use no operations at all).</p></div><div class="input-specification"><p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consisting of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". It is guaranteed that the string <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-it">correct</span>.</p></div><div class="output-specification"><p>Print one string — the minimum <span class="tex-font-style-it">correct</span> string that you can obtain from the given one.</p></div>

## Input

<p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the length of string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consisting of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". It is guaranteed that the string <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-it">correct</span>.</p>

## Output

<p>Print one string — the minimum <span class="tex-font-style-it">correct</span> string that you can obtain from the given one.</p>





```input1
4
1001

```




```input2
1
1

```




```output1
100

```




```output2
1

```



## Note

<p>In the first example you can obtain the answer by the following sequence of operations: "<span class="tex-font-style-tt">1001</span>" <img align="middle" class="tex-formula" src="file://n7efuWkI.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">1010</span>" <img align="middle" class="tex-formula" src="file://sqXk4xSL.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">1100</span>" <img align="middle" class="tex-formula" src="file://U3UE2vzj.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">100</span>".</p><p>In the second example you can't obtain smaller answer no matter what operations you use.</p>
