## Description

<div><center> <img class="tex-graphics" src="file://NtURXGgm.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>One morning the Cereal Guy found out that all his cereal flakes were gone. He found a note instead of them. It turned out that his smart roommate hid the flakes in one of <span class="tex-span"><i>n</i></span> boxes. The boxes stand in one row, they are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the left to the right. The roommate left hints like "Hidden to the left of the <span class="tex-span"><i>i</i></span>-th box" ("<span class="tex-font-style-tt">To the left of <span class="tex-span"><i>i</i></span></span>"), "Hidden to the right of the <span class="tex-span"><i>i</i></span>-th box" ("<span class="tex-font-style-tt">To the right of <span class="tex-span"><i>i</i></span></span>"). Such hints mean that there are no flakes in the <span class="tex-span"><i>i</i></span>-th box as well. The Cereal Guy wants to know the minimal number of boxes he necessarily needs to check to find the flakes considering all the hints. Or he wants to find out that the hints are contradictory and the roommate lied to him, that is, no box has the flakes.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>m</i> ≤ 1000</span>) which represent the number of boxes and the number of hints correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain hints like "<span class="tex-font-style-tt">To the left of <span class="tex-span"><i>i</i></span></span>" and "<span class="tex-font-style-tt">To the right of <span class="tex-span"><i>i</i></span></span>", where <span class="tex-span"><i>i</i></span> is integer (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). The hints may coincide.</p></div><div class="output-specification"><p>The answer should contain exactly one integer — the number of boxes that should necessarily be checked or "<span class="tex-font-style-tt">-1</span>" if the hints are contradictory.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>m</i> ≤ 1000</span>) which represent the number of boxes and the number of hints correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain hints like "<span class="tex-font-style-tt">To the left of <span class="tex-span"><i>i</i></span></span>" and "<span class="tex-font-style-tt">To the right of <span class="tex-span"><i>i</i></span></span>", where <span class="tex-span"><i>i</i></span> is integer (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). The hints may coincide.</p>

## Output

<p>The answer should contain exactly one integer — the number of boxes that should necessarily be checked or "<span class="tex-font-style-tt">-1</span>" if the hints are contradictory.</p>





```input1
2 1
To the left of 2

```




```input2
3 2
To the right of 1
To the right of 2

```




```input3
3 1
To the left of 3

```




```input4
3 2
To the left of 2
To the right of 1

```




```output1
1

```




```output2
1

```




```output3
2

```




```output4
-1

```


