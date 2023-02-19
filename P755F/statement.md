## Description

<div><p>It's Christmas time! PolandBall and his friends will be giving themselves gifts. There are <span class="tex-span"><i>n</i></span> Balls overall. Each Ball has someone for whom he should bring a present according to some permutation <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span> for all <span class="tex-span"><i>i</i></span>.</p><p>Unfortunately, Balls are quite clumsy. We know earlier that exactly <span class="tex-span"><i>k</i></span> of them will forget to bring their gift. A Ball number <span class="tex-span"><i>i</i></span> will get his present if the following two constraints will hold: </p><ol> <li> Ball number <span class="tex-span"><i>i</i></span> will bring the present he should give. </li><li> Ball <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub> = <i>i</i></span> will bring his present. </li></ol><p>What is minimum and maximum possible number of kids who will <span class="tex-font-style-bf">not</span> get their present if exactly <span class="tex-span"><i>k</i></span> Balls will forget theirs?</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>), representing the number of Balls and the number of Balls who will forget to bring their presents. </p><p>The second line contains the permutation <span class="tex-span"><i>p</i></span> of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the index of Ball who should get a gift from the <span class="tex-span"><i>i</i></span>-th Ball. For all <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span> holds.</p></div><div class="output-specification"><p>You should output two values&nbsp;— minimum and maximum possible number of Balls who will <span class="tex-font-style-bf">not</span> get their presents, in that order.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>), representing the number of Balls and the number of Balls who will forget to bring their presents. </p><p>The second line contains the permutation <span class="tex-span"><i>p</i></span> of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the index of Ball who should get a gift from the <span class="tex-span"><i>i</i></span>-th Ball. For all <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span> holds.</p>

## Output

<p>You should output two values&nbsp;— minimum and maximum possible number of Balls who will <span class="tex-font-style-bf">not</span> get their presents, in that order.</p>





```input1
5 2
3 4 1 5 2

```




```input2
10 1
2 3 4 5 6 7 8 9 10 1

```




```output1
2 4
```




```output2
2 2
```



## Note

<p>In the first sample, if the third and the first balls will forget to bring their presents, they will be th only balls not getting a present. Thus the minimum answer is <span class="tex-span">2</span>. However, if the first ans the second balls will forget to bring their presents, then only the fifth ball will get a present. So, the maximum answer is <span class="tex-span">4</span>.</p>
