## Description

<div><p>You are given a tetrahedron. Let's mark its vertices with letters <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>C</i></span> and <span class="tex-span"><i>D</i></span> correspondingly.</p><center> <img class="tex-graphics" src="file://xo1IrAhS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>An ant is standing in the vertex <span class="tex-span"><i>D</i></span> of the tetrahedron. The ant is quite active and he wouldn't stay idle. At each moment of time he makes a step from one vertex to another one along some edge of the tetrahedron. The ant just can't stand on one place.</p><p>You do not have to do much to solve the problem: your task is to count the number of ways in which the ant can go from the initial vertex <span class="tex-span"><i>D</i></span> to itself in exactly <span class="tex-span"><i>n</i></span> steps. In other words, you are asked to find out the number of different cyclic paths with the length of <span class="tex-span"><i>n</i></span> from vertex <span class="tex-span"><i>D</i></span> to itself. As the number can be quite large, you should print it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">7</sup></span>) — the required length of the cyclic path.</p></div><div class="output-specification"><p>Print the only integer — the required number of ways modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">7</sup></span>) — the required length of the cyclic path.</p>

## Output

<p>Print the only integer — the required number of ways modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
2

```




```input2
4

```




```output1
3

```




```output2
21

```



## Note

<p>The required paths in the first sample are: </p><ul> <li> <span class="tex-span"><i>D</i> - <i>A</i> - <i>D</i></span> </li><li> <span class="tex-span"><i>D</i> - <i>B</i> - <i>D</i></span> </li><li> <span class="tex-span"><i>D</i> - <i>C</i> - <i>D</i></span> </li></ul>
