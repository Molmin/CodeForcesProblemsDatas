## Description

<div><p>You have <span class="tex-span"><i>m</i> = <i>n</i>·<i>k</i></span> wooden staves. The <span class="tex-span"><i>i</i></span>-th stave has length <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. You have to assemble <span class="tex-span"><i>n</i></span> barrels consisting of <span class="tex-span"><i>k</i></span> staves each, you can use any <span class="tex-span"><i>k</i></span> staves to construct a barrel. Each stave must belong to exactly one barrel.</p><p>Let volume <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> of barrel <span class="tex-span"><i>j</i></span> be equal to the length of the <span class="tex-font-style-bf">minimal</span> stave in it.</p><center> <img class="tex-graphics" src="file://Buy2Zf0J.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You want to assemble exactly <span class="tex-span"><i>n</i></span> barrels with the maximal total sum of volumes. But you have to make them <span class="tex-font-style-it">equal enough</span>, so a difference between volumes of any pair of the resulting barrels must not exceed <span class="tex-span"><i>l</i></span>, i.e. <span class="tex-span">|<i>v</i><sub class="lower-index"><i>x</i></sub> - <i>v</i><sub class="lower-index"><i>y</i></sub>| ≤ <i>l</i></span> for any <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>y</i> ≤ <i>n</i></span>.</p><p>Print maximal total sum of volumes of <span class="tex-font-style-it">equal enough</span> barrels or <span class="tex-span">0</span> if it's impossible to satisfy the condition above.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>n</i>·<i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>m</i> = <i>n</i>·<i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — lengths of staves.</p></div><div class="output-specification"><p>Print single integer — maximal total sum of the volumes of barrels or <span class="tex-span">0</span> if it's impossible to construct exactly <span class="tex-span"><i>n</i></span> barrels satisfying the condition <span class="tex-span">|<i>v</i><sub class="lower-index"><i>x</i></sub> - <i>v</i><sub class="lower-index"><i>y</i></sub>| ≤ <i>l</i></span> for any <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>y</i> ≤ <i>n</i></span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>n</i>·<i>k</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>m</i> = <i>n</i>·<i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — lengths of staves.</p>

## Output

<p>Print single integer — maximal total sum of the volumes of barrels or <span class="tex-span">0</span> if it's impossible to construct exactly <span class="tex-span"><i>n</i></span> barrels satisfying the condition <span class="tex-span">|<i>v</i><sub class="lower-index"><i>x</i></sub> - <i>v</i><sub class="lower-index"><i>y</i></sub>| ≤ <i>l</i></span> for any <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>y</i> ≤ <i>n</i></span>.</p>





```input1
4 2 1
2 2 1 2 3 2 2 3

```




```input2
2 1 0
10 10

```




```input3
1 2 1
5 2

```




```input4
3 2 1
1 2 3 4 5 6

```




```output1
7

```




```output2
20

```




```output3
2

```




```output4
0

```



## Note

<p>In the first example you can form the following barrels: <span class="tex-span">[1, 2]</span>, <span class="tex-span">[2, 2]</span>, <span class="tex-span">[2, 3]</span>, <span class="tex-span">[2, 3]</span>.</p><p>In the second example you can form the following barrels: <span class="tex-span">[10]</span>, <span class="tex-span">[10]</span>.</p><p>In the third example you can form the following barrels: <span class="tex-span">[2, 5]</span>.</p><p>In the fourth example difference between volumes of barrels in any partition is at least <span class="tex-span">2</span> so it is impossible to make barrels equal enough.</p>
