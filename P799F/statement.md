## Description

<div><p>Butler Ostin wants to show Arkady that rows of odd number of fountains are beautiful, while rows of even number of fountains are not.</p><p>The butler wants to show Arkady <span class="tex-span"><i>n</i></span> gardens. Each garden is a row of <span class="tex-span"><i>m</i></span> cells, the <span class="tex-span"><i>i</i></span>-th garden has one fountain in each of the cells between <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> inclusive, and there are no more fountains in that garden. The issue is that some of the gardens contain even number of fountains, it is wrong to show them to Arkady.</p><p>Ostin wants to choose two integers <span class="tex-span"><i>a</i> ≤ <i>b</i></span> and show only part of each of the gardens that starts at cell <span class="tex-span"><i>a</i></span> and ends at cell <span class="tex-span"><i>b</i></span>. Of course, only such segments suit Ostin that each garden has either zero or odd number of fountains on this segment. Also, it is necessary that at least one garden has at least one fountain on the segment from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>.</p><p>Help Ostin to find the total length of all such segments, i.e. sum up the value <span class="tex-span">(<i>b</i> - <i>a</i> + 1)</span> for each suitable pair <span class="tex-span">(<i>a</i>, <i>b</i>)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of gardens and the length of each garden.</p><p><span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the bounds of the segment that contains fountains in the <span class="tex-span"><i>i</i></span>-th garden.</p></div><div class="output-specification"><p>Print one integer: the total length of all suitable segments.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of gardens and the length of each garden.</p><p><span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the bounds of the segment that contains fountains in the <span class="tex-span"><i>i</i></span>-th garden.</p>

## Output

<p>Print one integer: the total length of all suitable segments.</p>





```input1
1 5
2 4

```




```input2
3 6
2 4
3 6
4 4

```




```output1
23

```




```output2
19

```



## Note

<p>In the first example the following pairs suit Ostin: <span class="tex-span">(<i>a</i>, <i>b</i>)</span>: <span class="tex-span">(1, 2)</span>, <span class="tex-span">(1, 4)</span>, <span class="tex-span">(1, 5)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(2, 5)</span>, <span class="tex-span">(3, 3)</span>, <span class="tex-span">(4, 4)</span>, <span class="tex-span">(4, 5)</span>.</p><p>In the second example the following pairs suit Ostin: <span class="tex-span">(<i>a</i>, <i>b</i>)</span>: <span class="tex-span">(1, 2)</span>, <span class="tex-span">(1, 5)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(2, 5)</span>, <span class="tex-span">(3, 3)</span>, <span class="tex-span">(4, 4)</span>, <span class="tex-span">(4, 6)</span>, <span class="tex-span">(5, 5)</span>, <span class="tex-span">(6, 6)</span>.</p>
