## Description

<div><p>In a strategic computer game "Settlers II" one has to build defense structures to expand and protect the territory. Let's take one of these buildings. At the moment the defense structure accommodates exactly <span class="tex-span"><i>n</i></span> soldiers. Within this task we can assume that the number of soldiers in the defense structure won't either increase or decrease.</p><p>Every soldier has a rank — some natural number from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>. <span class="tex-span">1</span> stands for a private and <span class="tex-span"><i>k</i></span> stands for a general. The higher the rank of the soldier is, the better he fights. Therefore, the player profits from having the soldiers of the highest possible rank.</p><p>To increase the ranks of soldiers they need to train. But the soldiers won't train for free, and each training session requires one golden coin. On each training session all the <span class="tex-span"><i>n</i></span> soldiers are present.</p><p>At the end of each training session the soldiers' ranks increase as follows. First all the soldiers are divided into groups with the same rank, so that the least possible number of groups is formed. Then, within each of the groups where the soldiers below the rank <span class="tex-span"><i>k</i></span> are present, exactly one soldier increases his rank by one.</p><p>You know the ranks of all <span class="tex-span"><i>n</i></span> soldiers at the moment. Determine the number of golden coins that are needed to increase the ranks of all the soldiers to the rank <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>). They represent the number of soldiers and the number of different ranks correspondingly. The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-font-style-bf">in the non-decreasing order</span>. The <span class="tex-span"><i>i</i></span>-th of them, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, represents the rank of the <span class="tex-span"><i>i</i></span>-th soldier in the defense building (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>).</p></div><div class="output-specification"><p>Print a single integer — the number of golden coins needed to raise all the soldiers to the maximal rank.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>). They represent the number of soldiers and the number of different ranks correspondingly. The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-font-style-bf">in the non-decreasing order</span>. The <span class="tex-span"><i>i</i></span>-th of them, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, represents the rank of the <span class="tex-span"><i>i</i></span>-th soldier in the defense building (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>).</p>

## Output

<p>Print a single integer — the number of golden coins needed to raise all the soldiers to the maximal rank.</p>





```input1
4 4
1 2 2 3

```




```input2
4 3
1 1 1 1

```




```output1
4
```




```output2
5
```



## Note

<p>In the first example the ranks will be raised in the following manner:</p><p><span class="tex-font-style-tt">1 2 2 3</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">2 2 3 4</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">2 3 4 4</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">3 4 4 4</span> <span class="tex-span"> → </span> <span class="tex-font-style-tt">4 4 4 4</span></p><p>Thus totals to 4 training sessions that require 4 golden coins.</p>
