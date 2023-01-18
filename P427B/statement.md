## Description

<div><p>The prison of your city has <span class="tex-span"><i>n</i></span> prisoners. As the prison can't accommodate all of them, the city mayor has decided to transfer <span class="tex-span"><i>c</i></span> of the prisoners to a prison located in another city.</p><p>For this reason, he made the <span class="tex-span"><i>n</i></span> prisoners to stand in a line, with a number written on their chests. The number is the severity of the crime he/she has committed. The greater the number, the more severe his/her crime was.</p><p>Then, the mayor told you to choose the <span class="tex-span"><i>c</i></span> prisoners, who will be transferred to the other prison. He also imposed two conditions. They are,</p><ul> <li> The chosen <span class="tex-span"><i>c</i></span> prisoners has to form a contiguous segment of prisoners. </li><li> Any of the chosen prisoner's crime level should not be greater then <span class="tex-span"><i>t</i></span>. Because, that will make the prisoner a severe criminal and the mayor doesn't want to take the risk of his running away during the transfer. </li></ul><p>Find the number of ways you can choose the <span class="tex-span"><i>c</i></span> prisoners.</p></div><div class="input-specification"><p>The first line of input will contain three space separated integers <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>, <span class="tex-span"><i>t</i>&nbsp;(0 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup>)</span> and <span class="tex-span"><i>c</i>&nbsp;(1 ≤ <i>c</i> ≤ <i>n</i>)</span>. The next line will contain <span class="tex-span"><i>n</i></span> space separated integers, the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> integer is the severity <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> prisoner's crime. The value of crime severities will be non-negative and will not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. </p></div><div class="output-specification"><p>Print a single integer — the number of ways you can choose the <span class="tex-span"><i>c</i></span> prisoners.</p></div>

## Input

<p>The first line of input will contain three space separated integers <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>, <span class="tex-span"><i>t</i>&nbsp;(0 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup>)</span> and <span class="tex-span"><i>c</i>&nbsp;(1 ≤ <i>c</i> ≤ <i>n</i>)</span>. The next line will contain <span class="tex-span"><i>n</i></span> space separated integers, the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> integer is the severity <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> prisoner's crime. The value of crime severities will be non-negative and will not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. </p>

## Output

<p>Print a single integer — the number of ways you can choose the <span class="tex-span"><i>c</i></span> prisoners.</p>





```input1
4 3 3
2 3 1 1

```




```input2
1 1 1
2

```




```input3
11 4 2
2 2 0 7 3 2 2 4 9 1 4

```




```output1
2

```




```output2
0

```




```output3
6

```


