## Description

<div><p>Squirrel Liss lived in a forest peacefully, but unexpected trouble happens. Stones fall from a mountain. Initially Squirrel Liss occupies an interval <span class="tex-span">[0, 1]</span>. Next, <span class="tex-span"><i>n</i></span> stones will fall and Liss will escape from the stones. The stones are numbered from 1 to <span class="tex-span"><i>n</i></span> in order.</p><p>The stones always fall to the center of Liss's interval. When Liss occupies the interval <span class="tex-span">[<i>k</i> - <i>d</i>, <i>k</i> + <i>d</i>]</span> and a stone falls to <span class="tex-span"><i>k</i></span>, she will escape to the left or to the right. If she escapes to the left, her new interval will be <span class="tex-span">[<i>k</i> - <i>d</i>, <i>k</i>]</span>. If she escapes to the right, her new interval will be <span class="tex-span">[<i>k</i>, <i>k</i> + <i>d</i>]</span>.</p><p>You are given a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. If the <span class="tex-span"><i>i</i></span>-th character of <span class="tex-span"><i>s</i></span> is "<span class="tex-font-style-tt">l</span>" or "<span class="tex-font-style-tt">r</span>", when the <span class="tex-span"><i>i</i></span>-th stone falls Liss will escape to the left or to the right, respectively. Find the sequence of stones' numbers from left to right after all the <span class="tex-span"><i>n</i></span> stones falls.</p></div><div class="input-specification"><p>The input consists of only one line. The only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup></span>). Each character in <span class="tex-span"><i>s</i></span> will be either "<span class="tex-font-style-tt">l</span>" or "<span class="tex-font-style-tt">r</span>".</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines — on the <span class="tex-span"><i>i</i></span>-th line you should print the <span class="tex-span"><i>i</i></span>-th stone's number from the left.</p></div>

## Input

<p>The input consists of only one line. The only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup></span>). Each character in <span class="tex-span"><i>s</i></span> will be either "<span class="tex-font-style-tt">l</span>" or "<span class="tex-font-style-tt">r</span>".</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> lines — on the <span class="tex-span"><i>i</i></span>-th line you should print the <span class="tex-span"><i>i</i></span>-th stone's number from the left.</p>





```input1
llrlr

```




```input2
rrlll

```




```input3
lrlrr

```




```output1
3
5
4
2
1

```




```output2
1
2
5
4
3

```




```output3
2
4
5
3
1

```



## Note

<p>In the first example, the positions of stones 1, 2, 3, 4, 5 will be <img align="middle" class="tex-formula" src="file://ZavbkVgg.png" style="max-width: 100.0%;max-height: 100.0%;">, respectively. So you should print the sequence: 3, 5, 4, 2, 1.</p>
