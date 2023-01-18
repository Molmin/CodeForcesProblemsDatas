## Description

<div><p>Vasya is a school PE teacher. Unlike other PE teachers, Vasya doesn't like it when the students stand in line according to their height. Instead, he demands that the children stand in the following order: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the height of the <span class="tex-span"><i>i</i></span>-th student in the line and <span class="tex-span"><i>n</i></span> is the number of students in the line. The children find it hard to keep in mind this strange arrangement, and today they formed the line in the following order: <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, which upset Vasya immensely. Now Vasya wants to rearrange the children so that the resulting order is like this: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. During each move Vasya can swap two people who stand next to each other in the line. Help Vasya, find the sequence of swaps leading to the arrangement Vasya needs. It is not required to minimize the number of moves.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) which is the number of students. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) which represent the height of the student occupying the <span class="tex-span"><i>i</i></span>-th place must possess. The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) which represent the height of the student occupying the <span class="tex-span"><i>i</i></span>-th place in the initial arrangement. It is possible that some students possess similar heights. It is guaranteed that it is possible to arrange the children in the required order, i.e. <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> coincide as multisets.</p></div><div class="output-specification"><p>In the first line print an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) which is the number of moves. It is not required to minimize <span class="tex-span"><i>k</i></span> but it must not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. Then print <span class="tex-span"><i>k</i></span> lines each containing two space-separated integers. Line <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> + 1</span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) means that Vasya should swap students occupying places <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>) which is the number of students. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) which represent the height of the student occupying the <span class="tex-span"><i>i</i></span>-th place must possess. The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) which represent the height of the student occupying the <span class="tex-span"><i>i</i></span>-th place in the initial arrangement. It is possible that some students possess similar heights. It is guaranteed that it is possible to arrange the children in the required order, i.e. <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> coincide as multisets.</p>

## Output

<p>In the first line print an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) which is the number of moves. It is not required to minimize <span class="tex-span"><i>k</i></span> but it must not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>. Then print <span class="tex-span"><i>k</i></span> lines each containing two space-separated integers. Line <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> + 1</span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) means that Vasya should swap students occupying places <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p>





```input1
4
1 2 3 2
3 2 1 2

```




```input2
2
1 100500
1 100500

```




```output1
4
2 3
1 2
3 4
2 3

```




```output2
0

```


