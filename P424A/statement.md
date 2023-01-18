## Description

<div><p>Pasha has many hamsters and he makes them work out. Today, <span class="tex-span"><i>n</i></span> hamsters (<span class="tex-span"><i>n</i></span> is even) came to work out. The hamsters lined up and each hamster either sat down or stood up.</p><p>For another exercise, Pasha needs exactly <img align="middle" class="tex-formula" src="file://bohI6tNa.png" style="max-width: 100.0%;max-height: 100.0%;"> hamsters to stand up and the other hamsters to sit down. In one minute, Pasha can make some hamster ether sit down or stand up. How many minutes will he need to get what he wants if he acts optimally well?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200</span>; <span class="tex-span"><i>n</i></span> is even). The next line contains <span class="tex-span"><i>n</i></span> characters without spaces. These characters describe the hamsters' position: the <span class="tex-span"><i>i</i></span>-th character equals '<span class="tex-font-style-tt">X</span>', if the <span class="tex-span"><i>i</i></span>-th hamster in the row is standing, and '<span class="tex-font-style-tt">x</span>', if he is sitting.</p></div><div class="output-specification"><p>In the first line, print a single integer — the minimum required number of minutes. In the second line, print a string that describes the hamsters' position after Pasha makes the required changes. If there are multiple optimal positions, print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200</span>; <span class="tex-span"><i>n</i></span> is even). The next line contains <span class="tex-span"><i>n</i></span> characters without spaces. These characters describe the hamsters' position: the <span class="tex-span"><i>i</i></span>-th character equals '<span class="tex-font-style-tt">X</span>', if the <span class="tex-span"><i>i</i></span>-th hamster in the row is standing, and '<span class="tex-font-style-tt">x</span>', if he is sitting.</p>

## Output

<p>In the first line, print a single integer — the minimum required number of minutes. In the second line, print a string that describes the hamsters' position after Pasha makes the required changes. If there are multiple optimal positions, print any of them.</p>





```input1
4
xxXx

```




```input2
2
XX

```




```input3
6
xXXxXx

```




```output1
1
XxXx

```




```output2
1
xX

```




```output3
0
xXXxXx

```


