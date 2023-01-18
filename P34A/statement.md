## Description

<div><p><span class="tex-span"><i>n</i></span> soldiers stand in a circle. For each soldier his height <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is known. A reconnaissance unit can be made of such two <span class="tex-font-style-bf">neighbouring</span> soldiers, whose heights difference is minimal, i.e. <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>j</i></sub>|</span> is minimal. So each of them will be less noticeable with the other. Output any pair of soldiers that can form a reconnaissance unit.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — amount of soldiers. Then follow the heights of the soldiers in their order in the circle — <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). The soldier heights are given in clockwise or counterclockwise direction.</p></div><div class="output-specification"><p>Output two integers — indexes of <span class="tex-font-style-bf">neighbouring</span> soldiers, who should form a reconnaissance unit. If there are many optimum solutions, output any of them. Remember, that the soldiers stand in a circle.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — amount of soldiers. Then follow the heights of the soldiers in their order in the circle — <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). The soldier heights are given in clockwise or counterclockwise direction.</p>

## Output

<p>Output two integers — indexes of <span class="tex-font-style-bf">neighbouring</span> soldiers, who should form a reconnaissance unit. If there are many optimum solutions, output any of them. Remember, that the soldiers stand in a circle.</p>





```input1
5
10 12 13 15 10

```




```input2
4
10 20 30 40

```




```output1
5 1

```




```output2
1 2

```


