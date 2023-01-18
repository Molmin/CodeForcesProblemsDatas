## Description

<div><p>Petya likes horse racing very much. Horses numbered from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> take part in the races. Petya wants to evaluate the probability of victory; for some reason, to do that he needs to know the amount of nearly lucky horses' numbers. A <span class="tex-font-style-underline">nearly lucky</span> number is an integer number that has at least two lucky digits the distance between which does not exceed <span class="tex-span"><i>k</i></span>. Petya learned from some of his mates from Lviv that lucky digits are digits <span class="tex-span">4</span> and <span class="tex-span">7</span>. The distance between the digits is the absolute difference between their positions in the number of a horse. For example, if <span class="tex-span"><i>k</i> = 2</span>, then numbers <span class="tex-span">412395497</span>, <span class="tex-span">404</span>, <span class="tex-span">4070400000070004007</span> are nearly lucky and numbers <span class="tex-span">4</span>, <span class="tex-span">4123954997</span>, <span class="tex-span">4007000040070004007</span> are not.</p><p>Petya prepared <span class="tex-span"><i>t</i></span> intervals <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> and invented number <span class="tex-span"><i>k</i></span>, common for all of them. Your task is to find how many nearly happy numbers there are in each of these segments. Since the answers can be quite large, output them modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>t</i>, <i>k</i> ≤ 1000</span>) — the number of segments and the distance between the numbers correspondingly. Next <span class="tex-span"><i>t</i></span> lines contain pairs of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">1000</sup></span>). All numbers are given without the leading zeroes. Numbers in each line are separated by exactly one space character.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>t</i></span> lines. In each line print one integer — the answer for the corresponding segment modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>t</i>, <i>k</i> ≤ 1000</span>) — the number of segments and the distance between the numbers correspondingly. Next <span class="tex-span"><i>t</i></span> lines contain pairs of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">1000</sup></span>). All numbers are given without the leading zeroes. Numbers in each line are separated by exactly one space character.</p>

## Output

<p>Output <span class="tex-span"><i>t</i></span> lines. In each line print one integer — the answer for the corresponding segment modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
1 2
1 100

```




```input2
1 2
70 77

```




```input3
2 1
1 20
80 100

```




```output1
4

```




```output2
2

```




```output3
0
0

```



## Note

<p>In the first sample, the four nearly lucky numbers are 44, 47, 74, 77.</p><p>In the second sample, only 74 and 77 are in the given segment.</p>
