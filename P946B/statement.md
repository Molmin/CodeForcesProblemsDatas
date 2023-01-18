## Description

<div><p>You have two variables <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Consider the following sequence of actions performed with these variables:</p><ol><li> If <span class="tex-span"><i>a</i> = 0</span> or <span class="tex-span"><i>b</i> = 0</span>, end the process. Otherwise, go to step <span class="tex-span">2</span>;</li><li> If <span class="tex-span"><i>a</i> ≥ 2·<i>b</i></span>, then set the value of <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>a</i> - 2·<i>b</i></span>, and repeat step <span class="tex-span">1</span>. Otherwise, go to step <span class="tex-span">3</span>;</li><li> If <span class="tex-span"><i>b</i> ≥ 2·<i>a</i></span>, then set the value of <span class="tex-span"><i>b</i></span> to <span class="tex-span"><i>b</i> - 2·<i>a</i></span>, and repeat step <span class="tex-span">1</span>. Otherwise, end the process.</li></ol><p>Initially the values of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are positive integers, and so the process will be finite.</p><p>You have to determine the values of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> after the process ends.</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">18</sup></span>). <span class="tex-span"><i>n</i></span> is the initial value of variable <span class="tex-span"><i>a</i></span>, and <span class="tex-span"><i>m</i></span> is the initial value of variable <span class="tex-span"><i>b</i></span>.</p></div><div class="output-specification"><p>Print two integers — the values of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> after the end of the process.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">18</sup></span>). <span class="tex-span"><i>n</i></span> is the initial value of variable <span class="tex-span"><i>a</i></span>, and <span class="tex-span"><i>m</i></span> is the initial value of variable <span class="tex-span"><i>b</i></span>.</p>

## Output

<p>Print two integers — the values of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> after the end of the process.</p>





```input1
12 5

```




```input2
31 12

```




```output1
0 1

```




```output2
7 12

```



## Note

<p>Explanations to the samples:</p><ol><li> <span class="tex-span"><i>a</i> = 12</span>, <span class="tex-span"><i>b</i> = 5</span> <img align="middle" class="tex-formula" src="file://4X3DAsvc.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>a</i> = 2</span>, <span class="tex-span"><i>b</i> = 5</span> <img align="middle" class="tex-formula" src="file://mjCh2JLO.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>a</i> = 2</span>, <span class="tex-span"><i>b</i> = 1</span> <img align="middle" class="tex-formula" src="file://0GVDkQok.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>a</i> = 0</span>, <span class="tex-span"><i>b</i> = 1</span>;</li><li> <span class="tex-span"><i>a</i> = 31</span>, <span class="tex-span"><i>b</i> = 12</span> <img align="middle" class="tex-formula" src="file://elLhFupm.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>a</i> = 7</span>, <span class="tex-span"><i>b</i> = 12</span>.</li></ol>
