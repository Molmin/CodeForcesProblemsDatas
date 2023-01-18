## Description

<div><p>There is a sand trail in front of Alice's home.</p><p>In daytime, people walk over it and leave a footprint on the trail for their every single step. Alice cannot distinguish the order of the footprints, but she can tell whether each footprint is made by left foot or right foot. Also she's certain that all people are walking by alternating left foot and right foot.</p><p>For example, suppose that one person walked through the trail and left some footprints. The footprints are <span class="tex-font-style-tt">RRLRL</span> in order along the trail ('R' means right foot and 'L' means left foot). You might think the outcome of the footprints is strange. But in fact, some steps are resulting from walking backwards!</p><p>There are some possible order of steps that produce these footprints such as <span class="tex-span">1 → 3 → 2 → 5 → 4</span> or <span class="tex-span">2 → 3 → 4 → 5 → 1</span> (we suppose that the distance between two consecutive steps can be arbitrarily long). The number of backward steps from above two examples are <span class="tex-span">2</span> and <span class="tex-span">1</span> separately.</p><p>Alice is interested in these footprints. Whenever there is a person walking trough the trail, she takes a picture of all these footprints along the trail and erase all of them so that next person will leave a new set of footprints. We know that people walk by alternating right foot and left foot, but we don't know if the first step is made by left foot or right foot.</p><p>Alice wants to know the minimum possible number of backward steps made by a person. But it's a little hard. Please help Alice to calculate it. You also need to construct one possible history of these footprints.</p></div><div class="input-specification"><p>Only one line containing the string <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 100 000</span>) containing all footprints in order along the trail from entrance to exit.</p><p>It is guaranteed that there is at least one possible footprint history.</p></div><div class="output-specification"><p>You should output <span class="tex-span">2</span> lines.</p><p>The first line should contain a number denoting the minimum number of backward steps.</p><p>The second line should contain a permutation of integers from 1 to <span class="tex-span">|<i>S</i>|</span>. This permutation should denote the order of footprints that may possible be used by person walked there.</p><p>If there are several possible answers, you may output any of them.</p></div>

## Input

<p>Only one line containing the string <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ |<i>S</i>| ≤ 100 000</span>) containing all footprints in order along the trail from entrance to exit.</p><p>It is guaranteed that there is at least one possible footprint history.</p>

## Output

<p>You should output <span class="tex-span">2</span> lines.</p><p>The first line should contain a number denoting the minimum number of backward steps.</p><p>The second line should contain a permutation of integers from 1 to <span class="tex-span">|<i>S</i>|</span>. This permutation should denote the order of footprints that may possible be used by person walked there.</p><p>If there are several possible answers, you may output any of them.</p>





```input1
RRLRL

```




```input2
RLRLRLRLR

```




```input3
RRRRRLLLL

```




```output1
1
2 5 1 3 4

```




```output2
0
1 2 3 4 5 6 7 8 9

```




```output3
4
4 9 3 8 2 7 1 6 5

```



## Note

<p>For the first sample, one possible order is <span class="tex-span">2 → 5 → 1 → 3 → 4</span>, among them only the step <span class="tex-span">5 → 1</span> is backward step so the answer is <span class="tex-span">1</span>. </p><p>For the second example one possible order is just to follow the order of input, thus there are no backward steps. </p><p>For the third sample, there will be <span class="tex-span">4</span> backward steps because every step from L to R will be a backward step.</p>
