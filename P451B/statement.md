## Description

<div><p>Being a programmer, you like arrays a lot. For your birthday, your friends have given you an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> <span class="tex-font-style-bf">distinct</span> integers.</p><p>Unfortunately, the size of <span class="tex-span"><i>a</i></span> is too small. You want a bigger array! Your friends agree to give you a bigger array, but only if you are able to answer the following question correctly: is it possible to sort the array <span class="tex-span"><i>a</i></span> (in increasing order) by reversing <span class="tex-font-style-bf">exactly one</span> segment of <span class="tex-span"><i>a</i></span>? See definitions of segment and reversing in the notes.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers: <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">yes</span>" or "<span class="tex-font-style-tt">no</span>" (without quotes), depending on the answer.</p><p>If your answer is "<span class="tex-font-style-tt">yes</span>", then also print two space-separated integers denoting start and end (start must not be greater than end) indices of the segment to be reversed. If there are multiple ways of selecting these indices, print any of them.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers: <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print "<span class="tex-font-style-tt">yes</span>" or "<span class="tex-font-style-tt">no</span>" (without quotes), depending on the answer.</p><p>If your answer is "<span class="tex-font-style-tt">yes</span>", then also print two space-separated integers denoting start and end (start must not be greater than end) indices of the segment to be reversed. If there are multiple ways of selecting these indices, print any of them.</p>





```input1
3
3 2 1

```




```input2
4
2 1 3 4

```




```input3
4
3 1 2 4

```




```input4
2
1 2

```




```output1
yes
1 3

```




```output2
yes
1 2

```




```output3
no

```




```output4
yes
1 1

```



## Note

<p>Sample 1. You can reverse the entire array to get <span class="tex-span">[1, 2, 3]</span>, which is sorted.</p><p>Sample 3. No segment can be reversed such that the array will be sorted.</p><p><span class="tex-font-style-it">Definitions</span></p><p>A segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> of array <span class="tex-span"><i>a</i></span> is the sequence <span class="tex-span"><i>a</i>[<i>l</i>], <i>a</i>[<i>l</i> + 1], ..., <i>a</i>[<i>r</i>]</span>.</p><p>If you have an array <span class="tex-span"><i>a</i></span> of size <span class="tex-span"><i>n</i></span> and you reverse its segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, the array will become:</p><p><span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>l</i> - 2], <i>a</i>[<i>l</i> - 1], <i>a</i>[<i>r</i>], <i>a</i>[<i>r</i> - 1], ..., <i>a</i>[<i>l</i> + 1], <i>a</i>[<i>l</i>], <i>a</i>[<i>r</i> + 1], <i>a</i>[<i>r</i> + 2], ..., <i>a</i>[<i>n</i> - 1], <i>a</i>[<i>n</i>].</span></p>
