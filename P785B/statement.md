## Description

<div><p>Anton likes to play chess. Also he likes to do programming. No wonder that he decided to attend chess classes and programming classes.</p><p>Anton has <span class="tex-span"><i>n</i></span> variants when he will attend chess classes, <span class="tex-span"><i>i</i></span>-th variant is given by a period of time <span class="tex-span">(<i>l</i><sub class="lower-index">1, <i>i</i></sub>, <i>r</i><sub class="lower-index">1, <i>i</i></sub>)</span>. Also he has <span class="tex-span"><i>m</i></span> variants when he will attend programming classes, <span class="tex-span"><i>i</i></span>-th variant is given by a period of time <span class="tex-span">(<i>l</i><sub class="lower-index">2, <i>i</i></sub>, <i>r</i><sub class="lower-index">2, <i>i</i></sub>)</span>.</p><p>Anton needs to choose <span class="tex-font-style-bf">exactly one</span> of <span class="tex-span"><i>n</i></span> possible periods of time when he will attend chess classes and <span class="tex-font-style-bf">exactly one</span> of <span class="tex-span"><i>m</i></span> possible periods of time when he will attend programming classes. He wants to have a rest between classes, so from all the possible pairs of the periods he wants to choose the one where the distance between the periods is maximal.</p><p>The distance between periods <span class="tex-span">(<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>)</span> is the minimal possible distance between a point in the first period and a point in the second period, that is the minimal possible <span class="tex-span">|<i>i</i> - <i>j</i>|</span>, where <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> ≤ <i>i</i> ≤ <i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index">2</sub> ≤ <i>j</i> ≤ <i>r</i><sub class="lower-index">2</sub></span>. In particular, when the periods intersect, the distance between them is <span class="tex-span">0</span>.</p><p>Anton wants to know how much time his rest between the classes will last in the best case. Help Anton and find this number!</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000)</span>&nbsp;— the number of time periods when Anton can attend chess classes.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines of the input contains two integers <span class="tex-span"><i>l</i><sub class="lower-index">1, <i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">1, <i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index">1, <i>i</i></sub> ≤ <i>r</i><sub class="lower-index">1, <i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;— the <span class="tex-span"><i>i</i></span>-th variant of a period of time when Anton can attend chess classes.</p><p>The following line of the input contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 200 000)</span>&nbsp;— the number of time periods when Anton can attend programming classes.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines of the input contains two integers <span class="tex-span"><i>l</i><sub class="lower-index">2, <i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2, <i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index">2, <i>i</i></sub> ≤ <i>r</i><sub class="lower-index">2, <i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;— the <span class="tex-span"><i>i</i></span>-th variant of a period of time when Anton can attend programming classes.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximal possible distance between time periods.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000)</span>&nbsp;— the number of time periods when Anton can attend chess classes.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines of the input contains two integers <span class="tex-span"><i>l</i><sub class="lower-index">1, <i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">1, <i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index">1, <i>i</i></sub> ≤ <i>r</i><sub class="lower-index">1, <i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;— the <span class="tex-span"><i>i</i></span>-th variant of a period of time when Anton can attend chess classes.</p><p>The following line of the input contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 200 000)</span>&nbsp;— the number of time periods when Anton can attend programming classes.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines of the input contains two integers <span class="tex-span"><i>l</i><sub class="lower-index">2, <i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2, <i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index">2, <i>i</i></sub> ≤ <i>r</i><sub class="lower-index">2, <i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;— the <span class="tex-span"><i>i</i></span>-th variant of a period of time when Anton can attend programming classes.</p>

## Output

<p>Output one integer&nbsp;— the maximal possible distance between time periods.</p>





```input1
3
1 5
2 6
2 3
2
2 4
6 8

```




```input2
3
1 5
2 6
3 7
2
2 4
1 4

```




```output1
3

```




```output2
0

```



## Note

<p>In the first sample Anton can attend chess classes in the period <span class="tex-span">(2, 3)</span> and attend programming classes in the period <span class="tex-span">(6, 8)</span>. It's not hard to see that in this case the distance between the periods will be equal to <span class="tex-span">3</span>.</p><p>In the second sample if he chooses any pair of periods, they will intersect. So the answer is <span class="tex-span">0</span>.</p>
