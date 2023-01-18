## Description

<div><p>There is a fence in front of Polycarpus's home. The fence consists of <span class="tex-span"><i>n</i></span> planks of the same width which go one after another from left to right. The height of the <span class="tex-span"><i>i</i></span>-th plank is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> meters, distinct planks can have distinct heights.</p><center> <img class="tex-graphics" src="file://jEZNGaq0.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Fence for <span class="tex-span"><i>n</i> = 7</span> and <span class="tex-span"><i>h</i> = [1, 2, 6, 1, 1, 7, 1]</span></span> </center><p>Polycarpus has bought a posh piano and is thinking about how to get it into the house. In order to carry out his plan, he needs to take exactly <span class="tex-span"><i>k</i></span> consecutive planks from the fence. Higher planks are harder to tear off the fence, so Polycarpus wants to find such <span class="tex-span"><i>k</i></span> consecutive planks that the sum of their heights is minimal possible.</p><p>Write the program that finds the indexes of <span class="tex-span"><i>k</i></span> consecutive planks with minimal total height. Pay attention, the fence is not around Polycarpus's home, it is in front of home (in other words, the fence isn't cyclic).</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1.5·10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of planks in the fence and the width of the hole for the piano. The second line contains the sequence of integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the height of the <span class="tex-span"><i>i</i></span>-th plank of the fence.</p></div><div class="output-specification"><p>Print such integer <span class="tex-span"><i>j</i></span> that the sum of the heights of planks <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>j</i> + 1</span>, ..., <span class="tex-span"><i>j</i> + <i>k</i> - 1</span> is the minimum possible. If there are multiple such <span class="tex-span"><i>j</i></span>'s, print any of them.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1.5·10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of planks in the fence and the width of the hole for the piano. The second line contains the sequence of integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the height of the <span class="tex-span"><i>i</i></span>-th plank of the fence.</p>

## Output

<p>Print such integer <span class="tex-span"><i>j</i></span> that the sum of the heights of planks <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>j</i> + 1</span>, ..., <span class="tex-span"><i>j</i> + <i>k</i> - 1</span> is the minimum possible. If there are multiple such <span class="tex-span"><i>j</i></span>'s, print any of them.</p>





```input1
7 3
1 2 6 1 1 7 1

```




```output1
3

```



## Note

<p>In the sample, your task is to find three consecutive planks with the minimum sum of heights. In the given case three planks with indexes 3, 4 and 5 have the required attribute, their total height is 8.</p>
