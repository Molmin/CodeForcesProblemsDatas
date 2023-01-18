## Description

<div><p>Once upon a time a little frog whose name was Vasya decided to travel around his home swamp. Overall there are <span class="tex-span"><i>n</i></span> mounds on the swamp, located on one line. The distance between the neighboring mounds is one meter. Vasya wants to visit all the mounds in one day; besides, he wants to visit each one exactly once. For that he makes a route plan, to decide the order in which to jump on the mounds. Vasya can pick any mound as the first one. He thinks it boring to jump two times at the same distance. That's why he wants any two jumps on his route to have different lengths. Help Vasya the Frog and make the plan for him.</p></div><div class="input-specification"><p>The single line contains a number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>) which is the number of mounds.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which are the frog's route plan. </p><ul> <li> All the <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>'s should be mutually different. </li><li> All the <span class="tex-span">|<i>p</i><sub class="lower-index"><i>i</i></sub>–<i>p</i><sub class="lower-index"><i>i</i> + 1</sub>|</span>'s should be mutually different (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>). </li></ul><p>If there are several solutions, output any.</p></div>

## Input

<p>The single line contains a number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>) which is the number of mounds.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which are the frog's route plan. </p><ul> <li> All the <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>'s should be mutually different. </li><li> All the <span class="tex-span">|<i>p</i><sub class="lower-index"><i>i</i></sub>–<i>p</i><sub class="lower-index"><i>i</i> + 1</sub>|</span>'s should be mutually different (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>). </li></ul><p>If there are several solutions, output any.</p>





```input1
2

```




```input2
3

```




```output1
1 2
```




```output2
1 3 2
```


