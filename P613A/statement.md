## Description

<div><p>Peter got a new snow blower as a New Year present. Of course, Peter decided to try it immediately. After reading the instructions he realized that it does not work like regular snow blowing machines. In order to make it work, you need to tie it to some point that it does not cover, and then switch it on. As a result it will go along a circle around this point and will remove all the snow from its path.</p><p>Formally, we assume that Peter's machine is a polygon on a plane. Then, after the machine is switched on, it will make a circle around the point to which Peter tied it (this point lies strictly outside the polygon). That is, each of the points lying within or on the border of the polygon will move along the circular trajectory, with the center of the circle at the point to which Peter tied his machine.</p><p>Peter decided to tie his car to point <span class="tex-span"><i>P</i></span> and now he is wondering what is the area of ​​the region that will be cleared from snow. Help him.</p></div><div class="input-specification"><p>The first line of the input contains three integers&nbsp;— the number of vertices of the polygon <span class="tex-span"><i>n</i></span> (<img align="middle" class="tex-formula" src="file://2smUy8aM.png" style="max-width: 100.0%;max-height: 100.0%;">), and coordinates of point <span class="tex-span"><i>P</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers&nbsp;— coordinates of the vertices of the polygon in the clockwise or counterclockwise order. It is guaranteed that no three consecutive vertices lie on a common straight line.</p><p>All the numbers in the input are integers that do not exceed <span class="tex-span">1 000 000</span> in their absolute value.</p></div><div class="output-specification"><p>Print a single real value number&nbsp;— the area of the region that will be cleared. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://vGxa3WvQ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains three integers&nbsp;— the number of vertices of the polygon <span class="tex-span"><i>n</i></span> (<img align="middle" class="tex-formula" src="file://2smUy8aM.png" style="max-width: 100.0%;max-height: 100.0%;">), and coordinates of point <span class="tex-span"><i>P</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers&nbsp;— coordinates of the vertices of the polygon in the clockwise or counterclockwise order. It is guaranteed that no three consecutive vertices lie on a common straight line.</p><p>All the numbers in the input are integers that do not exceed <span class="tex-span">1 000 000</span> in their absolute value.</p>

## Output

<p>Print a single real value number&nbsp;— the area of the region that will be cleared. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://vGxa3WvQ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 0 0
0 1
-1 2
1 2

```




```input2
4 1 -1
0 0
1 2
2 0
1 1

```




```output1
12.566370614359172464

```




```output2
21.991148575128551812

```



## Note

<p>In the first sample snow will be removed from that area:</p><center> <img class="tex-graphics" src="file://eNWDxQzo.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center>
