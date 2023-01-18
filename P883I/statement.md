## Description

<div><p>Evlampiy has found one more cool application to process photos. However the application has certain limitations.</p><p>Each photo <span class="tex-span"><i>i</i></span> has a contrast <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. In order for the processing to be truly of high quality, the application must receive at least <span class="tex-span"><i>k</i></span> photos with contrasts which differ as little as possible.</p><p>Evlampiy already knows the contrast <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> for each of his <span class="tex-span"><i>n</i></span> photos. Now he wants to split the photos into groups, so that each group contains at least <span class="tex-span"><i>k</i></span> photos. As a result, each photo must belong to exactly one group.</p><p>He considers a processing time of the <span class="tex-span"><i>j</i></span>-th group to be the difference between the maximum and minimum values of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in the group. Because of multithreading the processing time of a division into groups is the maximum processing time among all groups.</p><p>Split <span class="tex-span"><i>n</i></span> photos into groups in a such way that the processing time of the division is the minimum possible, i.e. that the the maximum processing time over all groups as least as possible.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — number of photos and minimum size of a group.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the contrast of the <span class="tex-span"><i>i</i></span>-th photo.</p></div><div class="output-specification"><p>Print the minimal processing time of the division into groups.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — number of photos and minimum size of a group.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the contrast of the <span class="tex-span"><i>i</i></span>-th photo.</p>

## Output

<p>Print the minimal processing time of the division into groups.</p>





```input1
5 2
50 110 130 40 120

```




```input2
4 1
2 3 4 1

```




```output1
20

```




```output2
0

```



## Note

<p>In the first example the photos should be split into 2 groups: <span class="tex-span">[40, 50]</span> and <span class="tex-span">[110, 120, 130]</span>. The processing time of the first group is <span class="tex-span">10</span>, and the processing time of the second group is <span class="tex-span">20</span>. Maximum among <span class="tex-span">10</span> and <span class="tex-span">20</span> is <span class="tex-span">20</span>. It is impossible to split the photos into groups in a such way that the processing time of division is less than <span class="tex-span">20</span>.</p><p>In the second example the photos should be split into four groups, each containing one photo. So the minimal possible processing time of a division is <span class="tex-span">0</span>.</p>
