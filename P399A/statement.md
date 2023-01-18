## Description

<div><p>User ainta is making a web site. This time he is going to make a navigation of the pages. In his site, there are <span class="tex-span"><i>n</i></span> pages numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Assume that somebody is on the <span class="tex-span"><i>p</i></span>-th page now. The navigation will look like this:</p><center> <span class="tex-font-style-tt">&lt;&lt; <span class="tex-span"><i>p</i> - <i>k</i></span> <span class="tex-span"><i>p</i> - <i>k</i> + 1</span> <span class="tex-span">...</span> <span class="tex-span"><i>p</i> - 1</span> <span class="tex-span">(<i>p</i>)</span> <span class="tex-span"><i>p</i> + 1</span> <span class="tex-span">...</span> <span class="tex-span"><i>p</i> + <i>k</i> - 1</span> <span class="tex-span"><i>p</i> + <i>k</i></span> &gt;&gt;</span> </center><p>When someone clicks the button "<span class="tex-font-style-tt">&lt;&lt;</span>" he is redirected to page <span class="tex-span">1</span>, and when someone clicks the button "<span class="tex-font-style-tt">&gt;&gt;</span>" he is redirected to page <span class="tex-span"><i>n</i></span>. Of course if someone clicks on a number, he is redirected to the corresponding page.</p><p>There are some conditions in the navigation:</p><ul> <li> If page <span class="tex-span">1</span> is in the navigation, the button "<span class="tex-font-style-tt">&lt;&lt;</span>" must not be printed. </li><li> If page <span class="tex-span"><i>n</i></span> is in the navigation, the button "<span class="tex-font-style-tt">&gt;&gt;</span>" must not be printed. </li><li> If the page number is smaller than <span class="tex-span">1</span> or greater than <span class="tex-span"><i>n</i></span>, it must not be printed. </li></ul> &nbsp;<p>You can see some examples of the navigations. Make a program that prints the navigation.</p></div><div class="input-specification"><p>The first and the only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>; <span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)</p></div><div class="output-specification"><p>Print the proper navigation. Follow the format of the output from the test samples.</p></div>

## Input

<p>The first and the only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>; <span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)</p>

## Output

<p>Print the proper navigation. Follow the format of the output from the test samples.</p>





```input1
17 5 2

```




```input2
6 5 2

```




```input3
6 1 2

```




```input4
6 2 2

```




```input5
9 6 3

```




```input6
10 6 3

```




```input7
8 5 4

```




```output1
&lt;&lt; 3 4 (5) 6 7 &gt;&gt;
```




```output2
&lt;&lt; 3 4 (5) 6
```




```output3
(1) 2 3 &gt;&gt;
```




```output4
1 (2) 3 4 &gt;&gt;
```




```output5
&lt;&lt; 3 4 5 (6) 7 8 9
```




```output6
&lt;&lt; 3 4 5 (6) 7 8 9 &gt;&gt;
```




```output7
1 2 3 4 (5) 6 7 8
```


