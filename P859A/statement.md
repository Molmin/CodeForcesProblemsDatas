## Description

<div><p>This year, as in previous years, MemSQL is inviting the top 25 competitors from the Start[c]up qualification round to compete onsite for the final round. Not everyone who is eligible to compete onsite can afford to travel to the office, though. Initially the top 25 contestants are invited to come onsite. Each eligible contestant must either accept or decline the invitation. Whenever a contestant declines, the highest ranked contestant not yet invited is invited to take the place of the one that declined. This continues until 25 contestants have accepted invitations.</p><p>After the qualifying round completes, you know <span class="tex-span"><i>K</i></span> of the onsite finalists, as well as their qualifying ranks (which start at <span class="tex-span">1</span>, there are no ties). Determine the minimum possible number of contestants that declined the invitation to compete onsite in the final round.</p></div><div class="input-specification"><p>The first line of input contains <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>K</i> ≤ 25</span>), the number of onsite finalists you know. The second line of input contains <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>K</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), the qualifying ranks of the finalists you know. All these ranks are distinct.</p></div><div class="output-specification"><p>Print the minimum possible number of contestants that declined the invitation to compete onsite.</p></div>

## Input

<p>The first line of input contains <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>K</i> ≤ 25</span>), the number of onsite finalists you know. The second line of input contains <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>K</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), the qualifying ranks of the finalists you know. All these ranks are distinct.</p>

## Output

<p>Print the minimum possible number of contestants that declined the invitation to compete onsite.</p>





```input1
25
2 3 4 5 6 7 8 9 10 11 12 14 15 16 17 18 19 20 21 22 23 24 25 26 28

```




```input2
5
16 23 8 15 4

```




```input3
3
14 15 92

```




```output1
3

```




```output2
0

```




```output3
67

```



## Note

<p>In the first example, you know all 25 onsite finalists. The contestants who ranked <span class="tex-span">1</span>-st, <span class="tex-span">13</span>-th, and <span class="tex-span">27</span>-th must have declined, so the answer is <span class="tex-span">3</span>.</p>
