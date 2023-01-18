## Description

<div><p>An army of <span class="tex-span"><i>n</i></span> droids is lined up in one row. Each droid is described by <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of details of the <span class="tex-span"><i>i</i></span>-th type in this droid's mechanism. R2-D2 wants to destroy the sequence of consecutive droids of maximum length. He has <span class="tex-span"><i>m</i></span> weapons, the <span class="tex-span"><i>i</i></span>-th weapon can affect all the droids in the army by destroying one detail of the <span class="tex-span"><i>i</i></span>-th type (if the droid doesn't have details of this type, nothing happens to it). </p><p>A droid is considered to be destroyed when all of its details are destroyed. R2-D2 can make at most <span class="tex-span"><i>k</i></span> shots. How many shots from the weapon of what type should R2-D2 make to destroy the sequence of consecutive droids of maximum length?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 5</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of droids, the number of detail types and the number of available shots, respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines follow describing the droids. Each line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of details of the <span class="tex-span"><i>i</i></span>-th type for the respective robot.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> space-separated integers, where the <span class="tex-span"><i>i</i></span>-th number is the number of shots from the weapon of the <span class="tex-span"><i>i</i></span>-th type that the robot should make to destroy the subsequence of consecutive droids of the maximum length.</p><p>If there are multiple optimal solutions, print any of them. </p><p>It is not necessary to make exactly <span class="tex-span"><i>k</i></span> shots, the number of shots can be less.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 5</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of droids, the number of detail types and the number of available shots, respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines follow describing the droids. Each line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of details of the <span class="tex-span"><i>i</i></span>-th type for the respective robot.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> space-separated integers, where the <span class="tex-span"><i>i</i></span>-th number is the number of shots from the weapon of the <span class="tex-span"><i>i</i></span>-th type that the robot should make to destroy the subsequence of consecutive droids of the maximum length.</p><p>If there are multiple optimal solutions, print any of them. </p><p>It is not necessary to make exactly <span class="tex-span"><i>k</i></span> shots, the number of shots can be less.</p>





```input1
5 2 4
4 0
1 2
2 1
0 2
1 3

```




```input2
3 2 4
1 2
1 3
2 2

```




```output1
2 2

```




```output2
1 3

```



## Note

<p>In the first test the second, third and fourth droids will be destroyed. </p><p>In the second test the first and second droids will be destroyed.</p>
