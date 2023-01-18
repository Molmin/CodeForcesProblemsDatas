## Description

<div><p>Vladimir wants to modernize partitions in his office. To make the office more comfortable he decided to remove a partition and plant several bamboos in a row. He thinks it would be nice if there are <span class="tex-span"><i>n</i></span> bamboos in a row, and the <span class="tex-span"><i>i</i></span>-th from the left is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> meters high. </p><p>Vladimir has just planted <span class="tex-span"><i>n</i></span> bamboos in a row, each of which has height <span class="tex-span">0</span> meters right now, but they grow <span class="tex-span">1</span> meter each day. In order to make the partition nice Vladimir can cut each bamboo once at any height (no greater that the height of the bamboo), and then the bamboo will stop growing.</p><p>Vladimir wants to check the bamboos each <span class="tex-span"><i>d</i></span> days (i.e. <span class="tex-span"><i>d</i></span> days after he planted, then after <span class="tex-span">2<i>d</i></span> days and so on), and cut the bamboos that reached the required height. Vladimir wants the total length of bamboo parts he will cut off to be no greater than <span class="tex-span"><i>k</i></span> meters.</p><p>What is the maximum value <span class="tex-span"><i>d</i></span> he can choose so that he can achieve what he wants without cutting off more than <span class="tex-span"><i>k</i></span> meters of bamboo?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">11</sup></span>)&nbsp;— the number of bamboos and the maximum total length of cut parts, in meters.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the required heights of bamboos, in meters.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum value of <span class="tex-span"><i>d</i></span> such that Vladimir can reach his goal.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">11</sup></span>)&nbsp;— the number of bamboos and the maximum total length of cut parts, in meters.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the required heights of bamboos, in meters.</p>

## Output

<p>Print a single integer&nbsp;— the maximum value of <span class="tex-span"><i>d</i></span> such that Vladimir can reach his goal.</p>





```input1
3 4
1 3 5

```




```input2
3 40
10 30 50

```




```output1
3

```




```output2
32

```



## Note

<p>In the first example Vladimir can check bamboos each <span class="tex-span">3</span> days. Then he will cut the first and the second bamboos after <span class="tex-span">3</span> days, and the third bamboo after <span class="tex-span">6</span> days. The total length of cut parts is <span class="tex-span">2 + 0 + 1 = 3</span> meters.</p>
