## Description

<div><p>Let us define two functions <span class="tex-span"><i>f</i></span> and <span class="tex-span"><i>g</i></span> on positive integer numbers. </p><center> <img align="middle" class="tex-formula" src="file://iOdm6gUq.png" style="max-width: 100.0%;max-height: 100.0%;"><p><img align="middle" class="tex-formula" src="file://QK0IpAud.png" style="max-width: 100.0%;max-height: 100.0%;"> </p></center><p>You need to process <span class="tex-span"><i>Q</i></span> queries. In each query, you will be given three integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span>. You need to print the number of integers <span class="tex-span"><i>x</i></span> between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> inclusive, such that <span class="tex-span"><i>g</i>(<i>x</i>) = <i>k</i></span>. </p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>) representing the number of queries. </p><p><span class="tex-span"><i>Q</i></span> lines follow, each of which contains 3 integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>k</i> ≤ 9)</span>.</p></div><div class="output-specification"><p>For each query, print a single line containing the answer for that query.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>) representing the number of queries. </p><p><span class="tex-span"><i>Q</i></span> lines follow, each of which contains 3 integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>k</i> ≤ 9)</span>.</p>

## Output

<p>For each query, print a single line containing the answer for that query.</p>





```input1
4
22 73 9
45 64 6
47 55 7
2 62 4

```




```input2
4
82 94 6
56 67 4
28 59 9
39 74 4

```




```output1
1
4
0
8

```




```output2
3
1
1
5

```



## Note

<p>In the first example:</p><ul> <li> <span class="tex-span"><i>g</i>(33) = 9</span> as <span class="tex-span"><i>g</i>(33) = <i>g</i>(3 × 3) = <i>g</i>(9) = 9</span> </li><li> <span class="tex-span"><i>g</i>(47) = <i>g</i>(48) = <i>g</i>(60) = <i>g</i>(61) = 6</span> </li><li> There are no such integers between <span class="tex-span">47</span> and <span class="tex-span">55</span>. </li><li> <span class="tex-span"><i>g</i>(4) = <i>g</i>(14) = <i>g</i>(22) = <i>g</i>(27) = <i>g</i>(39) = <i>g</i>(40) = <i>g</i>(41) = <i>g</i>(58) = 4</span> </li></ul>
