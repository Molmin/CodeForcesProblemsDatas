## Description

<div><p>Someday, Drazil wanted to go on date with Varda. Drazil and Varda live on Cartesian plane. Drazil's home is located in point <span class="tex-span">(0, 0)</span> and Varda's home is located in point <span class="tex-span">(<i>a</i>, <i>b</i>)</span>. In each step, he can move in a unit distance in horizontal or vertical direction. In other words, from position <span class="tex-span">(<i>x</i>, <i>y</i>)</span> he can go to positions <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span> or <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span>. </p><p>Unfortunately, Drazil doesn't have sense of direction. So he randomly chooses the direction he will go to in each step. He may accidentally return back to his house during his travel. Drazil may even not notice that he has arrived to <span class="tex-span">(<i>a</i>, <i>b</i>)</span> and continue travelling. </p><p>Luckily, Drazil arrived to the position <span class="tex-span">(<i>a</i>, <i>b</i>)</span> successfully. Drazil said to Varda: "It took me exactly <span class="tex-span"><i>s</i></span> steps to travel from my house to yours". But Varda is confused about his words, she is not sure that it is possible to get from <span class="tex-span">(0, 0)</span> to <span class="tex-span">(<i>a</i>, <i>b</i>)</span> in exactly <span class="tex-span"><i>s</i></span> steps. Can you find out if it is possible for Varda?</p></div><div class="input-specification"><p>You are given three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>s</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ 2·10<sup class="upper-index">9</sup></span>) in a single line.</p></div><div class="output-specification"><p>If you think Drazil made a mistake and it is impossible to take exactly <span class="tex-span"><i>s</i></span> steps and get from his home to Varda's home, print "No" (without quotes).</p><p>Otherwise, print "Yes".</p></div>

## Input

<p>You are given three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>s</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ 2·10<sup class="upper-index">9</sup></span>) in a single line.</p>

## Output

<p>If you think Drazil made a mistake and it is impossible to take exactly <span class="tex-span"><i>s</i></span> steps and get from his home to Varda's home, print "No" (without quotes).</p><p>Otherwise, print "Yes".</p>





```input1
5 5 11

```




```input2
10 15 25

```




```input3
0 5 1

```




```input4
0 0 2

```




```output1
No

```




```output2
Yes

```




```output3
No

```




```output4
Yes

```



## Note

<p>In fourth sample case one possible route is: <img align="middle" class="tex-formula" src="file://XivvLupI.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
