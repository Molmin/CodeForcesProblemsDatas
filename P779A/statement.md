## Description

<div><p>In Berland each high school student is characterized by <span class="tex-font-style-it">academic performance</span> — integer value between <span class="tex-span">1</span> and <span class="tex-span">5</span>.</p><p>In high school <span class="tex-font-style-tt">0xFF</span> there are two groups of pupils: the group <span class="tex-span"><i>A</i></span> and the group <span class="tex-span"><i>B</i></span>. Each group consists of exactly <span class="tex-span"><i>n</i></span> students. An academic performance of each student is known — integer value between <span class="tex-span">1</span> and <span class="tex-span">5</span>.</p><p>The school director wants to redistribute students between groups so that each of the two groups has the same number of students whose academic performance is equal to <span class="tex-span">1</span>, the same number of students whose academic performance is <span class="tex-span">2</span> and so on. In other words, the purpose of the school director is to change the composition of groups, so that for each value of academic performance the numbers of students in both groups are equal.</p><p>To achieve this, there is a plan to produce a series of exchanges of students between groups. During the single exchange the director selects one student from the class <span class="tex-span"><i>A</i></span> and one student of class <span class="tex-span"><i>B</i></span>. After that, they both change their groups.</p><p>Print the least number of exchanges, in order to achieve the desired equal numbers of students for each academic performance.</p></div><div class="input-specification"><p>The first line of the input contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — number of students in both groups.</p><p>The second line contains sequence of integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is academic performance of the <span class="tex-span"><i>i</i></span>-th student of the group <span class="tex-span"><i>A</i></span>.</p><p>The third line contains sequence of integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is academic performance of the <span class="tex-span"><i>i</i></span>-th student of the group <span class="tex-span"><i>B</i></span>.</p></div><div class="output-specification"><p>Print the required minimum number of exchanges or <span class="tex-font-style-tt">-1</span>, if the desired distribution of students can not be obtained.</p></div>

## Input

<p>The first line of the input contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — number of students in both groups.</p><p>The second line contains sequence of integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is academic performance of the <span class="tex-span"><i>i</i></span>-th student of the group <span class="tex-span"><i>A</i></span>.</p><p>The third line contains sequence of integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 5</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is academic performance of the <span class="tex-span"><i>i</i></span>-th student of the group <span class="tex-span"><i>B</i></span>.</p>

## Output

<p>Print the required minimum number of exchanges or <span class="tex-font-style-tt">-1</span>, if the desired distribution of students can not be obtained.</p>





```input1
4
5 4 4 4
5 5 4 5

```




```input2
6
1 1 1 1 1 1
5 5 5 5 5 5

```




```input3
1
5
3

```




```input4
9
3 2 5 5 2 3 3 3 2
4 1 4 1 1 2 4 4 1

```




```output1
1

```




```output2
3

```




```output3
-1

```




```output4
4

```


