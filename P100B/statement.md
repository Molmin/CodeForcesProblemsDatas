## Description

<div><p>Kiana thinks two integers are friends if and only if one of them divides the other one. For example, 12 and 4 are friends, also 6 and 6 are friends too, but 120 and 36 are not.</p><p>A group of non-zero integers is called friendly, if each pair of its integers form a friend pair.</p><p>You are given a group of non-zero integers. See if they're friendly.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), where <span class="tex-span"><i>n</i></span> — the number of integers in the group.</p><p>The next line contains the elements, sorted in the non-decreasing order. The numbers are comma separated, they have at most 7 digits in their decimal notation and do not have any leading zeros.</p></div><div class="output-specification"><p>If the group is friendly write "<span class="tex-font-style-tt">FRIENDS</span>", else write "<span class="tex-font-style-tt">NOT FRIENDS</span>".</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>), where <span class="tex-span"><i>n</i></span> — the number of integers in the group.</p><p>The next line contains the elements, sorted in the non-decreasing order. The numbers are comma separated, they have at most 7 digits in their decimal notation and do not have any leading zeros.</p>

## Output

<p>If the group is friendly write "<span class="tex-font-style-tt">FRIENDS</span>", else write "<span class="tex-font-style-tt">NOT FRIENDS</span>".</p>





```input1
4
1,3,6,12

```




```input2
3
1,2,9

```




```output1
FRIENDS

```




```output2
NOT FRIENDS

```


