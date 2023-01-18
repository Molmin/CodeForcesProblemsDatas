## Description

<div><p>Today Patrick waits for a visit from his friend Spongebob. To prepare for the visit, Patrick needs to buy some goodies in two stores located near his house. There is a <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> meter long road between his house and the first shop and a <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span> meter long road between his house and the second shop. Also, there is a road of length <span class="tex-span"><i>d</i><sub class="lower-index">3</sub></span> directly connecting these two shops to each other. Help Patrick calculate the minimum distance that he needs to walk in order to go to both shops and return to his house.</p><center> <img class="tex-graphics" height="227px" src="file://l8musdNF.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>Patrick always starts at his house. He should visit both shops moving only along the three existing roads and return back to his house. He doesn't mind visiting the same shop or passing the same road multiple times. The only goal is to minimize the total distance traveled.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, <i>d</i><sub class="lower-index">3</sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the lengths of the paths. </p><ul> <li> <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> is the length of the path connecting Patrick's house and the first shop; </li><li> <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span> is the length of the path connecting Patrick's house and the second shop; </li><li> <span class="tex-span"><i>d</i><sub class="lower-index">3</sub></span> is the length of the path connecting both shops. </li></ul></div><div class="output-specification"><p>Print the minimum distance that Patrick will have to walk in order to visit both shops and return to his house.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, <i>d</i><sub class="lower-index">3</sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the lengths of the paths. </p><ul> <li> <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> is the length of the path connecting Patrick's house and the first shop; </li><li> <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span> is the length of the path connecting Patrick's house and the second shop; </li><li> <span class="tex-span"><i>d</i><sub class="lower-index">3</sub></span> is the length of the path connecting both shops. </li></ul>

## Output

<p>Print the minimum distance that Patrick will have to walk in order to visit both shops and return to his house.</p>





```input1
10 20 30

```




```input2
1 1 5

```




```output1
60

```




```output2
4

```



## Note

<p>The first sample is shown on the picture in the problem statement. One of the optimal routes is: house <img align="middle" class="tex-formula" src="file://nm7EcuIn.png" style="max-width: 100.0%;max-height: 100.0%;"> first shop <img align="middle" class="tex-formula" src="file://dLSzHEzl.png" style="max-width: 100.0%;max-height: 100.0%;"> second shop <img align="middle" class="tex-formula" src="file://qjWId9f0.png" style="max-width: 100.0%;max-height: 100.0%;"> house.</p><p>In the second sample one of the optimal routes is: house <img align="middle" class="tex-formula" src="file://fEMM4Fbb.png" style="max-width: 100.0%;max-height: 100.0%;"> first shop <img align="middle" class="tex-formula" src="file://uCsCykWf.png" style="max-width: 100.0%;max-height: 100.0%;"> house <img align="middle" class="tex-formula" src="file://GrEqgguG.png" style="max-width: 100.0%;max-height: 100.0%;"> second shop <img align="middle" class="tex-formula" src="file://LTEHS4OD.png" style="max-width: 100.0%;max-height: 100.0%;"> house.</p>
