## Description

<div><p>Snark and Philip are preparing the problemset for the upcoming pre-qualification round for semi-quarter-finals. They have a bank of <span class="tex-span"><i>n</i></span> problems, and they want to select any non-empty subset of it as a problemset.</p><p><span class="tex-span"><i>k</i></span> experienced teams are participating in the contest. Some of these teams already know some of the problems. To make the contest interesting for them, each of the teams should know at most half of the selected problems.</p><p>Determine if Snark and Philip can make an interesting problemset!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 4</span>)&nbsp;— the number of problems and the number of experienced teams.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i></span> integers, each equal to <span class="tex-span">0</span> or <span class="tex-span">1</span>. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span">1</span> if <span class="tex-span"><i>j</i></span>-th team knows <span class="tex-span"><i>i</i></span>-th problem and <span class="tex-span">0</span> otherwise.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity), if it is possible to make an interesting problemset, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each character either upper- or lowercase ("<span class="tex-font-style-tt">YeS</span>" and "<span class="tex-font-style-tt">yes</span>" are valid when the answer is "<span class="tex-font-style-tt">YES</span>").</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 4</span>)&nbsp;— the number of problems and the number of experienced teams.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i></span> integers, each equal to <span class="tex-span">0</span> or <span class="tex-span">1</span>. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span">1</span> if <span class="tex-span"><i>j</i></span>-th team knows <span class="tex-span"><i>i</i></span>-th problem and <span class="tex-span">0</span> otherwise.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity), if it is possible to make an interesting problemset, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each character either upper- or lowercase ("<span class="tex-font-style-tt">YeS</span>" and "<span class="tex-font-style-tt">yes</span>" are valid when the answer is "<span class="tex-font-style-tt">YES</span>").</p>





```input1
5 3
1 0 1
1 1 0
1 0 0
1 0 0
1 0 0

```




```input2
3 2
1 0
1 1
0 1

```




```output1
NO

```




```output2
YES

```



## Note

<p>In the first example you can't make any interesting problemset, because the first team knows all problems.</p><p>In the second example you can choose the first and the third problems.</p>
