## Description

<div><p>It's tough to be a superhero. And it's twice as tough to resist the supervillain who is cool at math. Suppose that you're an ordinary Batman in an ordinary city of Gotham. Your enemy Joker mined the building of the city administration and you only have several minutes to neutralize the charge. To do that you should enter the cancel code on the bomb control panel.</p><p>However, that mad man decided to give you a hint. This morning the mayor found a playing card under his pillow. There was a line written on the card:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://rBepolaC.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The bomb has a note saying "<span class="tex-span"><i>J</i>(<i>x</i>) = <i>A</i></span>", where <span class="tex-span"><i>A</i></span> is some positive integer. You suspect that the cancel code is some integer <span class="tex-span"><i>x</i></span> that meets the equation <span class="tex-span"><i>J</i>(<i>x</i>) = <i>A</i></span>. Now in order to decide whether you should neutralize the bomb or run for your life, you've got to count how many distinct positive integers <span class="tex-span"><i>x</i></span> meet this equation.</p></div><div class="input-specification"><p>The single line of the input contains a single integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>A</i> ≤ 10<sup class="upper-index">12</sup></span>).</p></div><div class="output-specification"><p>Print the number of solutions of the equation <span class="tex-span"><i>J</i>(<i>x</i>) = <i>A</i></span>.</p></div>

## Input

<p>The single line of the input contains a single integer <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>A</i> ≤ 10<sup class="upper-index">12</sup></span>).</p>

## Output

<p>Print the number of solutions of the equation <span class="tex-span"><i>J</i>(<i>x</i>) = <i>A</i></span>.</p>





```input1
3

```




```input2
24

```




```output1
1

```




```output2
3

```



## Note

<p>Record <span class="tex-span"><i>x</i>|<i>n</i></span> means that number <span class="tex-span"><i>n</i></span> divides number <span class="tex-span"><i>x</i></span>.</p><p><img align="middle" class="tex-formula" src="file://Jr5J9VcI.png" style="max-width: 100.0%;max-height: 100.0%;"> is defined as the largest positive integer that divides both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>In the first sample test the only suitable value of <span class="tex-span"><i>x</i></span> is <span class="tex-span">2</span>. Then <span class="tex-span"><i>J</i>(2) = 1 + 2</span>.</p><p>In the second sample test the following values of <span class="tex-span"><i>x</i></span> match:</p><ul> <li> <span class="tex-span"><i>x</i> = 14</span>, <span class="tex-span"><i>J</i>(14) = 1 + 2 + 7 + 14 = 24</span> </li><li> <span class="tex-span"><i>x</i> = 15</span>, <span class="tex-span"><i>J</i>(15) = 1 + 3 + 5 + 15 = 24</span> </li><li> <span class="tex-span"><i>x</i> = 23</span>, <span class="tex-span"><i>J</i>(23) = 1 + 23 = 24</span> </li></ul>
