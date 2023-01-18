## Description

<div><p>There are <span class="tex-span"><i>n</i></span> parliamentarians in Berland. They are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It happened that all parliamentarians with odd indices are Democrats and all parliamentarians with even indices are Republicans.</p><p>New parliament assembly hall is a rectangle consisting of <span class="tex-span"><i>a</i> × <i>b</i></span> chairs&nbsp;— <span class="tex-span"><i>a</i></span> rows of <span class="tex-span"><i>b</i></span> chairs each. Two chairs are considered neighbouring if they share as side. For example, chair number <span class="tex-span">5</span> in row number <span class="tex-span">2</span> is neighbouring to chairs number <span class="tex-span">4</span> and <span class="tex-span">6</span> in this row and chairs with number <span class="tex-span">5</span> in rows <span class="tex-span">1</span> and <span class="tex-span">3</span>. Thus, chairs have four neighbours in general, except for the chairs on the border of the hall</p><p>We know that if two parliamentarians from one political party (that is two Democrats or two Republicans) seat nearby they spent all time discussing internal party issues.</p><p>Write the program that given the number of parliamentarians and the sizes of the hall determine if there is a way to find a seat for any parliamentarian, such that no two members of the same party share neighbouring seats.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>)&nbsp;— the number of parliamentarians, the number of rows in the assembly hall and the number of seats in each row, respectively.</p></div><div class="output-specification"><p>If there is no way to assigns seats to parliamentarians in a proper way print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print the solution in <span class="tex-span"><i>a</i></span> lines, each containing <span class="tex-span"><i>b</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer of the <span class="tex-span"><i>i</i></span>-th line should be equal to the index of parliamentarian occupying this seat, or <span class="tex-span">0</span> if this seat should remain empty. If there are multiple possible solution, you may print any of them.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>)&nbsp;— the number of parliamentarians, the number of rows in the assembly hall and the number of seats in each row, respectively.</p>

## Output

<p>If there is no way to assigns seats to parliamentarians in a proper way print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print the solution in <span class="tex-span"><i>a</i></span> lines, each containing <span class="tex-span"><i>b</i></span> integers. The <span class="tex-span"><i>j</i></span>-th integer of the <span class="tex-span"><i>i</i></span>-th line should be equal to the index of parliamentarian occupying this seat, or <span class="tex-span">0</span> if this seat should remain empty. If there are multiple possible solution, you may print any of them.</p>





```input1
3 2 2

```




```input2
8 4 3

```




```input3
10 2 2

```




```output1
0 3
1 2

```




```output2
7 8 3
0 1 4
6 0 5
0 2 0

```




```output3
-1

```



## Note

<p>In the first sample there are many other possible solutions. For example, </p><pre class="verbatim">3 2<br>0 1<br></pre><p>and </p><pre class="verbatim">2 1<br>3 0<br></pre><p>The following assignment </p><pre class="verbatim">3 2<br>1 0<br></pre><p>is incorrect, because parliamentarians <span class="tex-span">1</span> and <span class="tex-span">3</span> are both from Democrats party but will occupy neighbouring seats.</p>
