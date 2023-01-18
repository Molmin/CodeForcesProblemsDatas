## Description

<div><p>In a building where Polycarp lives there are <span class="tex-font-style-it">equal</span> number of flats on each floor. Unfortunately, Polycarp don't remember how many flats are on each floor, but he remembers that the flats are numbered from <span class="tex-span">1</span> from lower to upper floors. That is, the first several flats are on the first floor, the next several flats are on the second and so on. Polycarp don't remember the total number of flats in the building, so you can consider the building to be infinitely high (i.e. there are infinitely many floors). Note that the floors are numbered from <span class="tex-span">1</span>.</p><p>Polycarp remembers on which floors several flats are located. It is guaranteed that this information is not self-contradictory. It means that there exists a building with equal number of flats on each floor so that the flats from Polycarp's memory have the floors Polycarp remembers.</p><p>Given this information, is it possible to restore the exact floor for flat <span class="tex-span"><i>n</i></span>? </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100</span>), where <span class="tex-span"><i>n</i></span> is the number of the flat you need to restore floor for, and <span class="tex-span"><i>m</i></span> is the number of flats in Polycarp's memory.</p><p><span class="tex-span"><i>m</i></span> lines follow, describing the Polycarp's memory: each of these lines contains a pair of integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), which means that the flat <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is on the <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>-th floor. All values <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>It is guaranteed that the given information is not self-contradictory.</p></div><div class="output-specification"><p>Print the number of the floor in which the <span class="tex-span"><i>n</i></span>-th flat is located, if it is possible to determine it in a unique way. Print <span class="tex-font-style-tt">-1</span> if it is not possible to uniquely restore this floor.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 100</span>), where <span class="tex-span"><i>n</i></span> is the number of the flat you need to restore floor for, and <span class="tex-span"><i>m</i></span> is the number of flats in Polycarp's memory.</p><p><span class="tex-span"><i>m</i></span> lines follow, describing the Polycarp's memory: each of these lines contains a pair of integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), which means that the flat <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is on the <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>-th floor. All values <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>It is guaranteed that the given information is not self-contradictory.</p>

## Output

<p>Print the number of the floor in which the <span class="tex-span"><i>n</i></span>-th flat is located, if it is possible to determine it in a unique way. Print <span class="tex-font-style-tt">-1</span> if it is not possible to uniquely restore this floor.</p>





```input1
10 3
6 2
2 1
7 3

```




```input2
8 4
3 1
6 2
5 2
2 1

```




```output1
4

```




```output2
-1

```



## Note

<p>In the first example the 6-th flat is on the 2-nd floor, while the 7-th flat is on the 3-rd, so, the 6-th flat is the last on its floor and there are 3 flats on each floor. Thus, the 10-th flat is on the 4-th floor.</p><p>In the second example there can be 3 or 4 flats on each floor, so we can't restore the floor for the 8-th flat.</p>
