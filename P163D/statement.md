## Description

<div><p>Vasya wants to buy a new refrigerator. He believes that a refrigerator should be a rectangular parallelepiped with integer edge lengths. Vasya calculated that for daily use he will need a refrigerator with volume of at least <span class="tex-span"><i>V</i></span>. Moreover, Vasya is a minimalist by nature, so the volume should be no more than <span class="tex-span"><i>V</i></span>, either — why take up extra space in the apartment? Having made up his mind about the volume of the refrigerator, Vasya faced a new challenge — for a fixed volume of <span class="tex-span"><i>V</i></span> the refrigerator must have the minimum surface area so that it is easier to clean.</p><p>The volume and the surface area of a refrigerator with edges <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> are equal to <span class="tex-span"><i>V</i> = <i>abc</i></span> and <span class="tex-span"><i>S</i> = 2(<i>ab</i> + <i>bc</i> + <i>ca</i>)</span>, correspondingly.</p><p>Given the volume <span class="tex-span"><i>V</i></span>, help Vasya find the integer lengths for the refrigerator's edges <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> so that the refrigerator's volume equals <span class="tex-span"><i>V</i></span> and its surface area <span class="tex-span"><i>S</i></span> is minimized.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 500</span>) — the number of data sets.</p><p>The description of <span class="tex-span"><i>t</i></span> data sets follows. Each set consists of a single integer <span class="tex-span"><i>V</i></span> (<span class="tex-span">2 ≤ <i>V</i> ≤ 10<sup class="upper-index">18</sup></span>), given by its factorization as follows.</p><p>Let <span class="tex-span"><i>V</i></span> = <span class="tex-span"><i>p</i><sub class="lower-index">1</sub><sup class="upper-index"><i>a</i><sub class="lower-index">1</sub></sup><i>p</i><sub class="lower-index">2</sub><sup class="upper-index"><i>a</i><sub class="lower-index">2</sub></sup>... <i>p</i><sub class="lower-index"><i>k</i></sub><sup class="upper-index"><i>a</i><sub class="lower-index"><i>k</i></sub></sup></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different prime numbers and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are positive integer powers. </p><p>Then the first line describing a data set contains a single positive integer <span class="tex-span"><i>k</i></span> — the number of different prime divisors of <span class="tex-span"><i>V</i></span>. Next <span class="tex-span"><i>k</i></span> lines contain prime numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and their powers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, separated by spaces. All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different, all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> lines, on the <span class="tex-span"><i>i</i></span>-th line print the answer to the <span class="tex-span"><i>i</i></span>-th data set as four space-separated integers: the minimum possible surface area <span class="tex-span"><i>S</i></span> and the corresponding edge lengths <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>. If there are multiple variants of the lengths of edges that give the minimum area, you are allowed to print any of them. You can print the lengths of the fridge's edges in any order.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 500</span>) — the number of data sets.</p><p>The description of <span class="tex-span"><i>t</i></span> data sets follows. Each set consists of a single integer <span class="tex-span"><i>V</i></span> (<span class="tex-span">2 ≤ <i>V</i> ≤ 10<sup class="upper-index">18</sup></span>), given by its factorization as follows.</p><p>Let <span class="tex-span"><i>V</i></span> = <span class="tex-span"><i>p</i><sub class="lower-index">1</sub><sup class="upper-index"><i>a</i><sub class="lower-index">1</sub></sup><i>p</i><sub class="lower-index">2</sub><sup class="upper-index"><i>a</i><sub class="lower-index">2</sub></sup>... <i>p</i><sub class="lower-index"><i>k</i></sub><sup class="upper-index"><i>a</i><sub class="lower-index"><i>k</i></sub></sup></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different prime numbers and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are positive integer powers. </p><p>Then the first line describing a data set contains a single positive integer <span class="tex-span"><i>k</i></span> — the number of different prime divisors of <span class="tex-span"><i>V</i></span>. Next <span class="tex-span"><i>k</i></span> lines contain prime numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and their powers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, separated by spaces. All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different, all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span>.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> lines, on the <span class="tex-span"><i>i</i></span>-th line print the answer to the <span class="tex-span"><i>i</i></span>-th data set as four space-separated integers: the minimum possible surface area <span class="tex-span"><i>S</i></span> and the corresponding edge lengths <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>. If there are multiple variants of the lengths of edges that give the minimum area, you are allowed to print any of them. You can print the lengths of the fridge's edges in any order.</p>





```input1
3
1
2 3
1
17 1
3
3 1
2 3
5 1

```




```output1
24 2 2 2
70 1 1 17
148 4 6 5

```



## Note

<p>In the first data set of the sample the fridge's volume <span class="tex-span"><i>V</i> = 2<sup class="upper-index">3</sup> = 8</span>, and the minimum surface area will be produced by the edges of equal length.</p><p>In the second data set the volume <span class="tex-span"><i>V</i> = 17</span>, and it can be produced by only one set of integer lengths.</p>
