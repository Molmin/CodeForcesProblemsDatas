## Description

<div><p>Limak is a little polar bear. According to some old traditions, his bear family prepared a New Year cake. And Limak likes cakes.</p><p>As you may know, a New Year cake is a strictly convex polygon with <span class="tex-span"><i>n</i></span> vertices.</p><p>Parents won't allow Limak to eat more than half of a cake because he would get sick. After some thinking they decided to cut a cake along one of <span class="tex-span"><i>n</i>·(<i>n</i> - 3) / 2</span> diagonals. Then Limak will get a non-greater piece.</p><p>Limak understands rules but he won't be happy if the second piece happens to be much bigger. Limak's disappointment will be equal to the difference between pieces' areas, multiplied by two. It can be proved that it will be integer for the given constraints.</p><p>There are <span class="tex-span"><i>n</i>·(<i>n</i> - 3) / 2</span> possible scenarios. Consider them all and find the sum of values of Limak's disappointment, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the number of vertices in the polygon denoting the cake.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th point.</p><p>It's guaranteed that all points are distinct, polygon is strictly convex and points are given in the clockwise order.</p></div><div class="output-specification"><p>Print the sum of values of Limak's disappointment over all possible scenarios modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the number of vertices in the polygon denoting the cake.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th point.</p><p>It's guaranteed that all points are distinct, polygon is strictly convex and points are given in the clockwise order.</p>

## Output

<p>Print the sum of values of Limak's disappointment over all possible scenarios modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
5
2 4
2 7
5 7
5 4
3 -2

```




```input2
4
-1000000000 -5000000
0 1234567
1 1
-5 -100000000

```




```input3
8
-10 0
-6 6
0 10
6 6
10 0
6 -6
0 -10
-6 -6

```




```output1
90

```




```output2
525185196

```




```output3
5216

```



## Note

<p>In the first sample possible values of Limak's disappointment are <span class="tex-span">0, 18, 18, 24, 30</span>.</p>
