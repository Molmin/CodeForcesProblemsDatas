## Description

<div><p>Santa Claus is the first who came to the Christmas Olympiad, and he is going to be the first to take his place at a desk! In the classroom there are <span class="tex-span"><i>n</i></span> lanes of <span class="tex-span"><i>m</i></span> desks each, and there are two working places at each of the desks. The lanes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the left to the right, the desks in a lane are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> starting from the blackboard. Note that the lanes go perpendicularly to the blackboard, not along it (see picture).</p><p>The organizers numbered all the working places from <span class="tex-span">1</span> to <span class="tex-span">2<i>nm</i></span>. The places are numbered by lanes (i.&nbsp;e. all the places of the first lane go first, then all the places of the second lane, and so on), in a lane the places are numbered starting from the nearest to the blackboard (i.&nbsp;e. from the first desk in the lane), at each desk, the place on the left is numbered before the place on the right.</p><center> <img class="tex-graphics" height="170px" src="file://XehXy8Cm.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   <span class="tex-font-size-small">The picture illustrates the first and the second samples.</span> </center><p>Santa Clause knows that his place has number <span class="tex-span"><i>k</i></span>. Help him to determine at which lane at which desk he should sit, and whether his place is on the left or on the right!</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2<i>nm</i></span>)&nbsp;— the number of lanes, the number of desks in each lane and the number of Santa Claus' place.</p></div><div class="output-specification"><p>Print two integers: the number of lane <span class="tex-span"><i>r</i></span>, the number of desk <span class="tex-span"><i>d</i></span>, and a character <span class="tex-span"><i>s</i></span>, which stands for the side of the desk Santa Claus. The character <span class="tex-span"><i>s</i></span> should be "<span class="tex-font-style-tt">L</span>", if Santa Clause should sit on the left, and "<span class="tex-font-style-tt">R</span>" if his place is on the right.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2<i>nm</i></span>)&nbsp;— the number of lanes, the number of desks in each lane and the number of Santa Claus' place.</p>

## Output

<p>Print two integers: the number of lane <span class="tex-span"><i>r</i></span>, the number of desk <span class="tex-span"><i>d</i></span>, and a character <span class="tex-span"><i>s</i></span>, which stands for the side of the desk Santa Claus. The character <span class="tex-span"><i>s</i></span> should be "<span class="tex-font-style-tt">L</span>", if Santa Clause should sit on the left, and "<span class="tex-font-style-tt">R</span>" if his place is on the right.</p>





```input1
4 3 9

```




```input2
4 3 24

```




```input3
2 4 4

```




```output1
2 2 L

```




```output2
4 3 R

```




```output3
1 2 R

```



## Note

<p>The first and the second samples are shown on the picture. The green place corresponds to Santa Claus' place in the first example, the blue place corresponds to Santa Claus' place in the second example.</p><p>In the third sample there are two lanes with four desks in each, and Santa Claus has the fourth place. Thus, his place is in the first lane at the second desk on the right.</p>
