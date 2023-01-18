## Description

<div><p>There are <span class="tex-span"><i>n</i></span> boys and <span class="tex-span"><i>m</i></span> girls studying in the class. They should stand in a line so that boys and girls alternated there as much as possible. Let's assume that positions in the line are indexed from left to right by numbers from 1 to <span class="tex-span"><i>n</i> + <i>m</i></span>. Then the number of integers <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i> + <i>m</i></span>) such that positions with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> contain children of different genders (position <span class="tex-span"><i>i</i></span> has a girl and position <span class="tex-span"><i>i</i> + 1</span> has a boy or vice versa) must be as large as possible. </p><p>Help the children and tell them how to form the line.</p></div><div class="input-specification"><p>The single line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>), separated by a space.</p></div><div class="output-specification"><p>Print a line of <span class="tex-span"><i>n</i> + <i>m</i></span> characters. Print on the <span class="tex-span"><i>i</i></span>-th position of the line character "<span class="tex-font-style-tt">B</span>", if the <span class="tex-span"><i>i</i></span>-th position of your arrangement should have a boy and "<span class="tex-font-style-tt">G</span>", if it should have a girl. </p><p>Of course, the number of characters "<span class="tex-font-style-tt">B</span>" should equal <span class="tex-span"><i>n</i></span> and the number of characters "<span class="tex-font-style-tt">G</span>" should equal <span class="tex-span"><i>m</i></span>. If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>The single line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>), separated by a space.</p>

## Output

<p>Print a line of <span class="tex-span"><i>n</i> + <i>m</i></span> characters. Print on the <span class="tex-span"><i>i</i></span>-th position of the line character "<span class="tex-font-style-tt">B</span>", if the <span class="tex-span"><i>i</i></span>-th position of your arrangement should have a boy and "<span class="tex-font-style-tt">G</span>", if it should have a girl. </p><p>Of course, the number of characters "<span class="tex-font-style-tt">B</span>" should equal <span class="tex-span"><i>n</i></span> and the number of characters "<span class="tex-font-style-tt">G</span>" should equal <span class="tex-span"><i>m</i></span>. If there are multiple optimal solutions, print any of them.</p>





```input1
3 3

```




```input2
4 2

```




```output1
GBGBGB

```




```output2
BGBGBB

```



## Note

<p>In the first sample another possible answer is <span class="tex-font-style-tt">BGBGBG</span>. </p><p>In the second sample answer <span class="tex-font-style-tt">BBGBGB</span> is also optimal.</p>
