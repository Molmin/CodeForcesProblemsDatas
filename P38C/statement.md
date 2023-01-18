## Description

<div><p>The blinds are known to consist of opaque horizontal stripes that can be rotated thus regulating the amount of light flowing in the room. There are <span class="tex-span"><i>n</i></span> blind stripes with the width of 1 in the factory warehouse for blind production. The problem is that all of them are spare details from different orders, that is, they may not have the same length (it is even possible for them to have different lengths)</p><p>Every stripe can be cut into two or more parts. The cuttings are made perpendicularly to the side along which the length is measured. Thus the cuttings do not change the width of a stripe but each of the resulting pieces has a lesser length (the sum of which is equal to the length of the initial stripe)</p><p>After all the cuttings the blinds are constructed through consecutive joining of several parts, similar in length, along sides, along which length is measured. Also, apart from the resulting pieces an initial stripe can be used as a blind if it hasn't been cut. It is forbidden to construct blinds in any other way.</p><p>Thus, if the blinds consist of <span class="tex-span"><i>k</i></span> pieces each <span class="tex-span"><i>d</i></span> in length, then they are of form of a rectangle of <span class="tex-span"><i>k</i> × <i>d</i></span> bourlemeters. </p><p>Your task is to find for what window possessing the largest possible area the blinds can be made from the given stripes if on technical grounds it is forbidden to use pieces shorter than <span class="tex-span"><i>l</i></span> bourlemeter. The window is of form of a rectangle with side lengths as positive integers.</p></div><div class="input-specification"><p>The first output line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>l</i> ≤ 100</span>). They are the number of stripes in the warehouse and the minimal acceptable length of a blind stripe in bourlemeters. The second line contains space-separated <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. They are the lengths of initial stripes in bourlemeters (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Print the single number — the maximal area of the window in square bourlemeters that can be completely covered. If no window with a positive area that can be covered completely without breaking any of the given rules exist, then print the single number <span class="tex-span">0</span>.</p></div>

## Input

<p>The first output line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>l</i> ≤ 100</span>). They are the number of stripes in the warehouse and the minimal acceptable length of a blind stripe in bourlemeters. The second line contains space-separated <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. They are the lengths of initial stripes in bourlemeters (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>Print the single number — the maximal area of the window in square bourlemeters that can be completely covered. If no window with a positive area that can be covered completely without breaking any of the given rules exist, then print the single number <span class="tex-span">0</span>.</p>





```input1
4 2
1 2 3 4

```




```input2
5 3
5 5 7 3 1

```




```input3
2 3
1 2

```




```output1
8

```




```output2
15

```




```output3
0

```



## Note

<p>In the first sample test the required window is <span class="tex-span">2 × 4</span> in size and the blinds for it consist of 4 parts, each 2 bourlemeters long. One of the parts is the initial stripe with the length of 2, the other one is a part of a cut stripe with the length of 3 and the two remaining stripes are parts of a stripe with the length of 4 cut in halves.</p>
