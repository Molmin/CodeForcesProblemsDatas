## Description

<div><p>Mad scientist Mike is building a time machine in his spare time. To finish the work, he needs a resistor with a certain resistance value.</p><p>However, all Mike has is lots of identical resistors with unit resistance <span class="tex-span"><i>R</i><sub class="lower-index">0</sub> = 1</span>. Elements with other resistance can be constructed from these resistors. In this problem, we will consider the following as elements: </p><ol> <li> one resistor; </li><li> an element and <span class="tex-font-style-bf">one</span> resistor plugged in sequence; </li><li> an element and <span class="tex-font-style-bf">one</span> resistor plugged in parallel. </li></ol><center> <img class="tex-graphics" src="file://cyn0hKIj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>With the consecutive connection the resistance of the new element equals <span class="tex-span"><i>R</i> = <i>R</i><sub class="lower-index"><i>e</i></sub> + <i>R</i><sub class="lower-index">0</sub></span>. With the parallel connection the resistance of the new element equals <img align="middle" class="tex-formula" src="file://CAPhPaZU.png" style="max-width: 100.0%;max-height: 100.0%;">. In this case <span class="tex-span"><i>R</i><sub class="lower-index"><i>e</i></sub></span> equals the resistance of the element being connected.</p><p>Mike needs to assemble an element with a resistance equal to the fraction <img align="middle" class="tex-formula" src="file://eZO6YHnO.png" style="max-width: 100.0%;max-height: 100.0%;">. Determine the smallest possible number of resistors he needs to make such an element.</p></div><div class="input-specification"><p>The single input line contains two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>). It is guaranteed that the fraction <img align="middle" class="tex-formula" src="file://dYI1k5Ds.png" style="max-width: 100.0%;max-height: 100.0%;"> is irreducible. It is guaranteed that a solution always exists.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is recommended to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The single input line contains two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>). It is guaranteed that the fraction <img align="middle" class="tex-formula" src="file://dYI1k5Ds.png" style="max-width: 100.0%;max-height: 100.0%;"> is irreducible. It is guaranteed that a solution always exists.</p>

## Output

<p>Print a single number — the answer to the problem.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is recommended to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
1 1

```




```input2
3 2

```




```input3
199 200

```




```output1
1

```




```output2
3

```




```output3
200

```



## Note

<p>In the first sample, one resistor is enough.</p><p>In the second sample one can connect the resistors in parallel, take the resulting element and connect it to a third resistor consecutively. Then, we get an element with resistance <img align="middle" class="tex-formula" src="file://uHJxIjQT.png" style="max-width: 100.0%;max-height: 100.0%;">. We cannot make this element using two resistors.</p>
