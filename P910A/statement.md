## Description

<div><p>A frog lives on the axis <span class="tex-span"><i>Ox</i></span> and needs to reach home which is in the point <span class="tex-span"><i>n</i></span>. She starts from the point <span class="tex-span">1</span>. The frog can jump to the right at a distance not more than <span class="tex-span"><i>d</i></span>. So, after she jumped from the point <span class="tex-span"><i>x</i></span> she can reach the point <span class="tex-span"><i>x</i> + <i>a</i></span>, where <span class="tex-span"><i>a</i></span> is an integer from <span class="tex-span">1</span> to <span class="tex-span"><i>d</i></span>.</p><p>For each point from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> is known if there is a lily flower in it. The frog can jump only in points with a lilies. Guaranteed that there are lilies in the points <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>.</p><p>Determine the minimal number of jumps that the frog needs to reach home which is in the point <span class="tex-span"><i>n</i></span> from the point <span class="tex-span">1</span>. Consider that initially the frog is in the point <span class="tex-span">1</span>. If the frog can not reach home, print <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>n</i> - 1</span>) — the point, which the frog wants to reach, and the maximal length of the frog jump.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of zeros and ones. If a character of the string <span class="tex-span"><i>s</i></span> equals to zero, then in the corresponding point there is no lily flower. In the other case, in the corresponding point there is a lily flower. Guaranteed that the first and the last characters of the string <span class="tex-span"><i>s</i></span> equal to one.</p></div><div class="output-specification"><p>If the frog can not reach the home, print <span class="tex-font-style-tt">-1</span>.</p><p>In the other case, print the minimal number of jumps that the frog needs to reach the home which is in the point <span class="tex-span"><i>n</i></span> from the point <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ <i>n</i> - 1</span>) — the point, which the frog wants to reach, and the maximal length of the frog jump.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of zeros and ones. If a character of the string <span class="tex-span"><i>s</i></span> equals to zero, then in the corresponding point there is no lily flower. In the other case, in the corresponding point there is a lily flower. Guaranteed that the first and the last characters of the string <span class="tex-span"><i>s</i></span> equal to one.</p>

## Output

<p>If the frog can not reach the home, print <span class="tex-font-style-tt">-1</span>.</p><p>In the other case, print the minimal number of jumps that the frog needs to reach the home which is in the point <span class="tex-span"><i>n</i></span> from the point <span class="tex-span">1</span>.</p>





```input1
8 4
10010101

```




```input2
4 2
1001

```




```input3
8 4
11100101

```




```input4
12 3
101111100101

```




```output1
2

```




```output2
-1

```




```output3
3

```




```output4
4

```



## Note

<p>In the first example the from can reach home in two jumps: the first jump from the point <span class="tex-span">1</span> to the point <span class="tex-span">4</span> (the length of the jump is three), and the second jump from the point <span class="tex-span">4</span> to the point <span class="tex-span">8</span> (the length of the jump is four).</p><p>In the second example the frog can not reach home, because to make it she need to jump on a distance three, but the maximum length of her jump equals to two.</p>
