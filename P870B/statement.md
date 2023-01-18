## Description

<div><p>You are given an array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> consisting of <span class="tex-span"><i>n</i></span> integers, and an integer <span class="tex-span"><i>k</i></span>. You have to split the array into exactly <span class="tex-span"><i>k</i></span> non-empty subsegments. You'll then compute the minimum integer on each subsegment, and take the maximum integer over the <span class="tex-span"><i>k</i></span> obtained minimums. What is the maximum possible integer you can get?</p><p>Definitions of subsegment and array splitting are given in notes.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤  10<sup class="upper-index">5</sup></span>) — the size of the array <span class="tex-span"><i>a</i></span> and the number of subsegments you have to split the array to.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup>  ≤  <i>a</i><sub class="lower-index"><i>i</i></sub> ≤  10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print single integer — the maximum possible integer you can get if you split the array into <span class="tex-span"><i>k</i></span> non-empty subsegments and take maximum of minimums on the subsegments.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤  10<sup class="upper-index">5</sup></span>) — the size of the array <span class="tex-span"><i>a</i></span> and the number of subsegments you have to split the array to.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup>  ≤  <i>a</i><sub class="lower-index"><i>i</i></sub> ≤  10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print single integer — the maximum possible integer you can get if you split the array into <span class="tex-span"><i>k</i></span> non-empty subsegments and take maximum of minimums on the subsegments.</p>





```input1
5 2
1 2 3 4 5

```




```input2
5 1
-4 -5 -3 -2 -1

```




```output1
5

```




```output2
-5

```



## Note

<p>A subsegment <span class="tex-span">[<i>l</i>,  <i>r</i>]</span> (<span class="tex-span"><i>l</i> ≤ <i>r</i></span>) of array <span class="tex-span"><i>a</i></span> is the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>,  <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>,  ...,  <i>a</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>Splitting of array <span class="tex-span"><i>a</i></span> of <span class="tex-span"><i>n</i></span> elements into <span class="tex-span"><i>k</i></span> subsegments <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span>, <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>]</span>, ..., <span class="tex-span">[<i>l</i><sub class="lower-index"><i>k</i></sub>, <i>r</i><sub class="lower-index"><i>k</i></sub>]</span> (<span class="tex-span"><i>l</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub> = <i>n</i></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>i</i> - 1</sub> + 1</span> for all <span class="tex-span"><i>i</i> &gt; 1</span>) is <span class="tex-span"><i>k</i></span> sequences <span class="tex-span">(<i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index">1</sub></sub>, ..., <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index">1</sub></sub>), ..., (<i>a</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>k</i></sub></sub>, ..., <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>k</i></sub></sub>)</span>.</p><p>In the first example you should split the array into subsegments <span class="tex-span">[1, 4]</span> and <span class="tex-span">[5, 5]</span> that results in sequences <span class="tex-span">(1, 2, 3, 4)</span> and <span class="tex-span">(5)</span>. The minimums are <span class="tex-span"><i>min</i>(1, 2, 3, 4) = 1</span> and <span class="tex-span"><i>min</i>(5) = 5</span>. The resulting maximum is <span class="tex-span"><i>max</i>(1, 5) = 5</span>. It is obvious that you can't reach greater result.</p><p>In the second example the only option you have is to split the array into one subsegment <span class="tex-span">[1, 5]</span>, that results in one sequence <span class="tex-span">( - 4,  - 5,  - 3,  - 2,  - 1)</span>. The only minimum is <span class="tex-span"><i>min</i>( - 4,  - 5,  - 3,  - 2,  - 1) =  - 5</span>. The resulting maximum is <span class="tex-span"> - 5</span>.</p>
