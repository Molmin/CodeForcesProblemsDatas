## Description

<div><p>A schoolboy Petya studies square equations. The equations that are included in the school curriculum, usually look simple: </p><center class="tex-equation"><span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 2<i>bx</i> + <i>c</i> = 0</span></center> where <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> are natural numbers.<p>Petya noticed that some equations have two real roots, some of them have only one root and some equations don't have real roots at all. Moreover it turned out that several different square equations can have a common root.</p><p>Petya is interested in how many different real roots have all the equations of the type described above for all the possible pairs of numbers <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> such that <span class="tex-span">1 ≤ <i>b</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>. Help Petya find that number.</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000000</span>).</p></div><div class="output-specification"><p>Print a single number which is the number of real roots of the described set of equations.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000000</span>).</p>

## Output

<p>Print a single number which is the number of real roots of the described set of equations.</p>





```input1
3 3

```




```input2
1 2

```




```output1
12

```




```output2
1

```



## Note

<p>In the second test from the statement the following equations are analysed:</p><p> <span class="tex-span"><i>b</i> = 1</span>, <span class="tex-span"><i>c</i> = 1</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 2<i>x</i> + 1 = 0</span>; The root is <span class="tex-span"><i>x</i> =  - 1</span></p><p> <span class="tex-span"><i>b</i> = 1</span>, <span class="tex-span"><i>c</i> = 2</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 2<i>x</i> + 2 = 0</span>; No roots</p><p> Overall there's one root</p><p>In the second test the following equations are analysed:</p><p> <span class="tex-span"><i>b</i> = 1</span>, <span class="tex-span"><i>c</i> = 1</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 2<i>x</i> + 1 = 0</span>; The root is <span class="tex-span"><i>x</i> =  - 1</span></p><p> <span class="tex-span"><i>b</i> = 1</span>, <span class="tex-span"><i>c</i> = 2</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 2<i>x</i> + 2 = 0</span>; No roots</p><p> <span class="tex-span"><i>b</i> = 1</span>, <span class="tex-span"><i>c</i> = 3</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 2<i>x</i> + 3 = 0</span>; No roots</p><p> <span class="tex-span"><i>b</i> = 2</span>, <span class="tex-span"><i>c</i> = 1</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 4<i>x</i> + 1 = 0</span>; The roots are <img align="middle" class="tex-formula" src="file://RP90uzQB.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p> <span class="tex-span"><i>b</i> = 2</span>, <span class="tex-span"><i>c</i> = 2</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 4<i>x</i> + 2 = 0</span>; The roots are <img align="middle" class="tex-formula" src="file://znVdHocy.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p> <span class="tex-span"><i>b</i> = 2</span>, <span class="tex-span"><i>c</i> = 3</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 4<i>x</i> + 3 = 0</span>; The roots are <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> =  - 3, <i>x</i><sub class="lower-index">2</sub> =  - 1</span></p><p> <span class="tex-span"><i>b</i> = 3</span>, <span class="tex-span"><i>c</i> = 1</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 6<i>x</i> + 1 = 0</span>; The roots are <img align="middle" class="tex-formula" src="file://4aGZuIhz.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p> <span class="tex-span"><i>b</i> = 3</span>, <span class="tex-span"><i>c</i> = 2</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 6<i>x</i> + 2 = 0</span>; The roots are <img align="middle" class="tex-formula" src="file://6AlBxsZS.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p> <span class="tex-span"><i>b</i> = 3</span>, <span class="tex-span"><i>c</i> = 3</span>: <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + 6<i>x</i> + 3 = 0</span>; The roots are <img align="middle" class="tex-formula" src="file://yb4SJ302.png" style="max-width: 100.0%;max-height: 100.0%;"> Overall there are <span class="tex-span">13</span> roots and as the root <span class="tex-span"> - 1</span> is repeated twice, that means there are <span class="tex-span">12</span> different roots.</p>
