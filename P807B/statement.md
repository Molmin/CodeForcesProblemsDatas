## Description

<div><p>Not so long ago the Codecraft-17 contest was held on Codeforces. The top 25 participants, and additionally random 25 participants out of those who got into top 500, will receive a Codeforces T-shirt.</p><p>Unfortunately, you didn't manage to get into top 25, but you got into top 500, taking place <span class="tex-span"><i>p</i></span>.</p><p>Now the elimination round of 8VC Venture Cup 2017 is being held. It has been announced that the Codecraft-17 T-shirt winners will be chosen as follows. Let <span class="tex-span"><i>s</i></span> be the number of points of the winner of the elimination round of 8VC Venture Cup 2017. Then the following pseudocode will be executed: </p><pre class="verbatim"><br>i := (s div 50) mod 475<br>repeat 25 times:<br>    i := (i * 96 + 42) mod 475<br>    print (26 + i)<br></pre><p>Here "<span class="tex-font-style-tt">div</span>" is the integer division operator, "<span class="tex-font-style-tt">mod</span>" is the modulo (the remainder of division) operator.</p><p>As the result of pseudocode execution, 25 integers between 26 and 500, inclusive, will be printed. These will be the numbers of places of the participants who get the Codecraft-17 T-shirts. It is guaranteed that the 25 printed integers will be pairwise distinct for any value of <span class="tex-span"><i>s</i></span>.</p><p>You're in the lead of the elimination round of 8VC Venture Cup 2017, having <span class="tex-span"><i>x</i></span> points. You believe that having at least <span class="tex-span"><i>y</i></span> points in the current round will be enough for victory.</p><p>To change your final score, you can make any number of successful and unsuccessful hacks. A successful hack brings you 100 points, an unsuccessful one takes 50 points from you. It's difficult to do successful hacks, though.</p><p>You want to win the current round and, at the same time, ensure getting a Codecraft-17 T-shirt. What is the smallest number of <span class="tex-font-style-bf">successful</span> hacks you have to do to achieve that?</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">26 ≤ <i>p</i> ≤ 500</span>; <span class="tex-span">1 ≤ <i>y</i> ≤ <i>x</i> ≤ 20000</span>)&nbsp;— your place in Codecraft-17, your current score in the elimination round of 8VC Venture Cup 2017, and the smallest number of points you consider sufficient for winning the current round.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the smallest number of successful hacks you have to do in order to both win the elimination round of 8VC Venture Cup 2017 and ensure getting a Codecraft-17 T-shirt.</p><p>It's guaranteed that your goal is achievable for any valid input data.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">26 ≤ <i>p</i> ≤ 500</span>; <span class="tex-span">1 ≤ <i>y</i> ≤ <i>x</i> ≤ 20000</span>)&nbsp;— your place in Codecraft-17, your current score in the elimination round of 8VC Venture Cup 2017, and the smallest number of points you consider sufficient for winning the current round.</p>

## Output

<p>Output a single integer&nbsp;— the smallest number of successful hacks you have to do in order to both win the elimination round of 8VC Venture Cup 2017 and ensure getting a Codecraft-17 T-shirt.</p><p>It's guaranteed that your goal is achievable for any valid input data.</p>





```input1
239 10880 9889

```




```input2
26 7258 6123

```




```input3
493 8000 8000

```




```input4
101 6800 6500

```




```input5
329 19913 19900

```




```output1
0

```




```output2
2

```




```output3
24

```




```output4
0

```




```output5
8

```



## Note

<p>In the first example, there is no need to do any hacks since 10880 points already bring the T-shirt to the 239-th place of Codecraft-17 (that is, you). In this case, according to the pseudocode, the T-shirts will be given to the participants at the following places: </p><pre class="verbatim"><br>475 422 84 411 453 210 157 294 146 188 420 367 29 356 398 155 102 239 91 133 365 312 449 301 343<br></pre><p>In the second example, you have to do two successful and one unsuccessful hack to make your score equal to 7408.</p><p>In the third example, you need to do as many as 24 successful hacks to make your score equal to 10400.</p><p>In the fourth example, it's sufficient to do 6 unsuccessful hacks (and no successful ones) to make your score equal to 6500, which is just enough for winning the current round and also getting the T-shirt.</p>
