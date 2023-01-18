## Description

<div><p>Today you are going to lead a group of elven archers to defend the castle that is attacked by an army of angry orcs. Three sides of the castle are protected by impassable mountains and the remaining side is occupied by a long wall that is split into <span class="tex-span"><i>n</i></span> sections. At this moment there are exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> archers located at the <span class="tex-span"><i>i</i></span>-th section of this wall. You know that archer who stands at section <span class="tex-span"><i>i</i></span> can shoot orcs that attack section located at distance not exceeding <span class="tex-span"><i>r</i></span>, that is all such sections <span class="tex-span"><i>j</i></span> that <span class="tex-span">|<i>i</i> - <i>j</i>| ≤ <i>r</i></span>. In particular, <span class="tex-span"><i>r</i> = 0</span> means that archers are only capable of shooting at orcs who attack section <span class="tex-span"><i>i</i></span>.</p><p>Denote as <span class="tex-font-style-underline">defense level</span> of section <span class="tex-span"><i>i</i></span> the total number of archers who can shoot at the orcs attacking this section. <span class="tex-font-style-underline">Reliability</span> of the defense plan is the minimum value of defense level of individual wall section.</p><p>There is a little time left till the attack so you can't redistribute archers that are already located at the wall. However, there is a reserve of <span class="tex-span"><i>k</i></span> archers that you can distribute among wall sections in arbitrary way. You would like to achieve maximum possible reliability of the defence plan.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>, <span class="tex-span">0 ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of sections of the wall, the maximum distance to other section archers can still shoot and the number of archers yet to be distributed along the wall. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the current number of archers at each section.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the maximum possible value of defense plan reliability, i.e. the maximum possible value of minimum defense level if we distribute <span class="tex-span"><i>k</i></span> additional archers optimally.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>, <span class="tex-span">0 ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of sections of the wall, the maximum distance to other section archers can still shoot and the number of archers yet to be distributed along the wall. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the current number of archers at each section.</p>

## Output

<p>Print one integer&nbsp;— the maximum possible value of defense plan reliability, i.e. the maximum possible value of minimum defense level if we distribute <span class="tex-span"><i>k</i></span> additional archers optimally.</p>





```input1
5 0 6
5 4 3 4 9

```




```input2
4 2 0
1 2 3 4

```




```input3
5 1 1
2 1 2 1 2

```




```output1
5

```




```output2
6

```




```output3
3

```


