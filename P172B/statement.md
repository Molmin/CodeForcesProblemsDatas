## Description

<div><p>Polycarpus has recently got interested in sequences of pseudorandom numbers. He learned that many programming languages generate such sequences in a similar way: <img align="middle" class="tex-formula" src="file://PzNeJRes.png" style="max-width: 100.0%;max-height: 100.0%;"> (for <span class="tex-span"><i>i</i> ≥ 1</span>). Here <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>m</i></span> are constants, fixed for the given realization of the pseudorandom numbers generator, <span class="tex-span"><i>r</i><sub class="lower-index">0</sub></span> is the so-called <span class="tex-span"><i>randseed</i></span> (this value can be set from the program using functions like <span class="tex-font-style-tt">RandSeed(r)</span> or <span class="tex-font-style-tt">srand(n)</span>), and <img align="middle" class="tex-formula" src="file://gDAFi1Py.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the operation of taking the remainder of division.</p><p>For example, if <span class="tex-span"><i>a</i> = 2, <i>b</i> = 6, <i>m</i> = 12, <i>r</i><sub class="lower-index">0</sub> = 11</span>, the generated sequence will be: <span class="tex-span">4, 2, 10, 2, 10, 2, 10, 2, 10, 2, 10, ...</span>.</p><p>Polycarpus realized that any such sequence will sooner or later form a cycle, but the cycle may occur not in the beginning, so there exist a preperiod and a period. The example above shows a preperiod equal to 1 and a period equal to 2.</p><p>Your task is to find the period of a sequence defined by the given values of <span class="tex-span"><i>a</i>, <i>b</i>, <i>m</i></span> and <span class="tex-span"><i>r</i><sub class="lower-index">0</sub></span>. Formally, you have to find such minimum positive integer <span class="tex-span"><i>t</i></span>, for which exists such positive integer <span class="tex-span"><i>k</i></span>, that for any <span class="tex-span"><i>i</i> ≥ <i>k</i></span>: <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>i</i> + <i>t</i></sub></span>.</p></div><div class="input-specification"><p>The single line of the input contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>r</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>a</i>, <i>b</i> ≤ 1000, 0 ≤ <i>r</i><sub class="lower-index">0</sub> &lt; <i>m</i></span>), separated by single spaces.</p></div><div class="output-specification"><p>Print a single integer — the period of the sequence.</p></div>

## Input

<p>The single line of the input contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>r</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>a</i>, <i>b</i> ≤ 1000, 0 ≤ <i>r</i><sub class="lower-index">0</sub> &lt; <i>m</i></span>), separated by single spaces.</p>

## Output

<p>Print a single integer — the period of the sequence.</p>





```input1
2 6 12 11

```




```input2
2 3 5 1

```




```input3
3 6 81 9

```




```output1
2

```




```output2
4

```




```output3
1

```



## Note

<p>The first sample is described above. </p><p>In the second sample the sequence is (starting from the first element): <span class="tex-span">0, 3, 4, 1, 0, 3, 4, 1, 0, ...</span></p><p>In the third sample the sequence is (starting from the first element): <span class="tex-span">33, 24, 78, 78, 78, 78, ...</span></p>
