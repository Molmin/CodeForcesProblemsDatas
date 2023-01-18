## Description

<div><p>Pasha and Akim were making a forest map — the lawns were the graph's vertexes and the roads joining the lawns were its edges. They decided to encode the number of laughy mushrooms on every lawn in the following way: on every edge between two lawns they wrote two numbers, the greatest common divisor (GCD) and the least common multiple (LCM) of the number of mushrooms on these lawns. But one day Pasha and Akim had an argument about the laughy mushrooms and tore the map. Pasha was left with just some part of it, containing only <span class="tex-span"><i>m</i></span> roads. Your task is to help Pasha — use the map he has to restore the number of mushrooms on every lawn. As the result is not necessarily unique, help Pasha to restore any one or report that such arrangement of mushrooms does not exist. It is guaranteed that the numbers on the roads on the initial map were no less that <span class="tex-span">1</span> and did not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://IqAEl649.png" style="max-width: 100.0%;max-height: 100.0%;">) which are the numbers of lawns and roads we know about. Each of the following <span class="tex-span"><i>m</i></span> lines contains four numbers which are the numbers of lawns the road connects, the GCD and the LCM of the numbers of mushrooms on these lawns (<span class="tex-span">1 ≤ <i>GCD</i>, <i>LCM</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It is guaranteed, that no road connects lawn to itself, and no two lawns are connected by more than one road.</p></div><div class="output-specification"><p>The answer should contain "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" on the first line, saying whether it is possible or not to perform the arrangement. If the answer is "<span class="tex-font-style-tt">YES</span>", print on the following line <span class="tex-span"><i>n</i></span> numbers which are the numbers of mushrooms on the corresponding lawns.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://IqAEl649.png" style="max-width: 100.0%;max-height: 100.0%;">) which are the numbers of lawns and roads we know about. Each of the following <span class="tex-span"><i>m</i></span> lines contains four numbers which are the numbers of lawns the road connects, the GCD and the LCM of the numbers of mushrooms on these lawns (<span class="tex-span">1 ≤ <i>GCD</i>, <i>LCM</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It is guaranteed, that no road connects lawn to itself, and no two lawns are connected by more than one road.</p>

## Output

<p>The answer should contain "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" on the first line, saying whether it is possible or not to perform the arrangement. If the answer is "<span class="tex-font-style-tt">YES</span>", print on the following line <span class="tex-span"><i>n</i></span> numbers which are the numbers of mushrooms on the corresponding lawns.</p>





```input1
1 0

```




```input2
2 1
1 2 1 3

```




```input3
3 2
3 2 1 2
3 1 1 10

```




```input4
2 1
1 2 3 7

```




```output1
YES
1
```




```output2
YES
1 3
```




```output3
YES
5 1 2
```




```output4
NO

```


