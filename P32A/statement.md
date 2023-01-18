## Description

<div><p>According to the regulations of Berland's army, a reconnaissance unit should consist of exactly two soldiers. Since these two soldiers shouldn't differ much, their heights can differ by at most <span class="tex-span"><i>d</i></span> centimeters. Captain Bob has <span class="tex-span"><i>n</i></span> soldiers in his detachment. Their heights are <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> centimeters. Some soldiers are of the same height. Bob wants to know, how many ways exist to form a reconnaissance unit of two soldiers from his detachment.</p><p>Ways <span class="tex-span">(1, 2)</span> and <span class="tex-span">(2, 1)</span> should be regarded as different.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) — amount of soldiers in Bob's detachment and the maximum allowed height difference respectively. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — heights of all the soldiers in Bob's detachment. These numbers don't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Output one number — amount of ways to form a reconnaissance unit of two soldiers, whose height difference doesn't exceed <span class="tex-span"><i>d</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) — amount of soldiers in Bob's detachment and the maximum allowed height difference respectively. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — heights of all the soldiers in Bob's detachment. These numbers don't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Output one number — amount of ways to form a reconnaissance unit of two soldiers, whose height difference doesn't exceed <span class="tex-span"><i>d</i></span>.</p>





```input1
5 10
10 20 50 60 65

```




```input2
5 1
55 30 29 31 55

```




```output1
6

```




```output2
6

```


