## Description

<div><p>There are <span class="tex-span"><i>n</i></span> student groups at the university. During the study day, each group can take no more than <span class="tex-span">7</span> classes. Seven time slots numbered from <span class="tex-span">1</span> to <span class="tex-span">7</span> are allocated for the classes.</p><p>The schedule on Monday is known for each group, i. e. time slots when group will have classes are known.</p><p>Your task is to determine the minimum number of rooms needed to hold classes for all groups on Monday. Note that one room can hold at most one group class in a single time slot.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of groups. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains a sequence consisting of <span class="tex-span">7</span> zeroes and ones — the schedule of classes on Monday for a group. If the symbol in a position equals to <span class="tex-span">1</span> then the group has class in the corresponding time slot. In the other case, the group has no class in the corresponding time slot.</p></div><div class="output-specification"><p>Print minimum number of rooms needed to hold all groups classes on Monday.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of groups. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains a sequence consisting of <span class="tex-span">7</span> zeroes and ones — the schedule of classes on Monday for a group. If the symbol in a position equals to <span class="tex-span">1</span> then the group has class in the corresponding time slot. In the other case, the group has no class in the corresponding time slot.</p>

## Output

<p>Print minimum number of rooms needed to hold all groups classes on Monday.</p>





```input1
2
0101010
1010101

```




```input2
3
0101011
0011001
0110111

```




```output1
1

```




```output2
3

```



## Note

<p>In the first example one room is enough. It will be occupied in each of the seven time slot by the first group or by the second group.</p><p>In the second example three rooms is enough, because in the seventh time slot all three groups have classes.</p>
