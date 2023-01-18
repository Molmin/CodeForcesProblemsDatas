## Description

<div><p>As Valeric and Valerko were watching one of the last Euro Championship games in a sports bar, they broke a mug. Of course, the guys paid for it but the barman said that he will let them watch football in his bar only if they help his son complete a programming task. The task goes like that.</p><p>Let's consider a set of functions of the following form: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://rX76hk3T.png" style="max-width: 100.0%;max-height: 100.0%;"></center> Let's define a sum of <span class="tex-span"><i>n</i></span> functions <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>(<i>x</i>), ..., <i>y</i><sub class="lower-index"><i>n</i></sub>(<i>x</i>)</span> of the given type as function <span class="tex-span"><i>s</i>(<i>x</i>) = <i>y</i><sub class="lower-index">1</sub>(<i>x</i>) + ... + <i>y</i><sub class="lower-index"><i>n</i></sub>(<i>x</i>)</span> for any <span class="tex-span"><i>x</i></span>. It's easy to show that in this case the graph <span class="tex-span"><i>s</i>(<i>x</i>)</span> is a polyline. You are given <span class="tex-span"><i>n</i></span> functions of the given type, your task is to find the number of angles that do not equal 180 degrees, in the graph <span class="tex-span"><i>s</i>(<i>x</i>)</span>, that is the sum of the given functions.<p>Valeric and Valerko really want to watch the next Euro Championship game, so they asked you to help them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of functions. Each of the following <span class="tex-span"><i>n</i></span> lines contains two space-separated integer numbers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> that determine the <span class="tex-span"><i>i</i></span>-th function.</p></div><div class="output-specification"><p>Print a single number — the number of angles that do not equal 180 degrees in the graph of the polyline that equals the sum of the given functions.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of functions. Each of the following <span class="tex-span"><i>n</i></span> lines contains two space-separated integer numbers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> that determine the <span class="tex-span"><i>i</i></span>-th function.</p>

## Output

<p>Print a single number — the number of angles that do not equal 180 degrees in the graph of the polyline that equals the sum of the given functions.</p>





```input1
1
1 0

```




```input2
3
1 0
0 2
-1 1

```




```input3
3
-2 -4
1 7
-5 1

```




```output1
1

```




```output2
2

```




```output3
3

```


