## Description

<div><p>Vasya the carpenter has an estate that is separated from the wood by a fence. The fence consists of <span class="tex-span"><i>n</i></span> planks put in a line. The fence is not closed in a circle. The planks are numbered from left to right from 1 to <span class="tex-span"><i>n</i></span>, the <span class="tex-span"><i>i</i></span>-th plank is of height <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. All planks have the same width, the lower edge of each plank is located at the ground level.</p><p>Recently a local newspaper "Malevich and Life" wrote that the most fashionable way to decorate a fence in the summer is to draw a fuchsia-colored rectangle on it, the lower side of the rectangle must be located at the lower edge of the fence.</p><p>Vasya is delighted with this idea! He immediately bought some fuchsia-colored paint and began to decide what kind of the rectangle he should paint. Vasya is sure that the rectangle should cover <span class="tex-span"><i>k</i></span> consecutive planks. In other words, he will paint planks number <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>x</i> + 1</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i> + <i>k</i> - 1</span> for some <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i> - <i>k</i> + 1)</span>. He wants to paint the rectangle of maximal area, so the rectangle height equals <span class="tex-span"><i>min</i> <i>a</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span"><i>x</i> ≤ <i>i</i> ≤ <i>x</i> + <i>k</i> - 1</span>, <span class="tex-span"><i>x</i></span> is the number of the first colored plank.</p><p>Vasya has already made up his mind that the rectangle width can be equal to one of numbers of the sequence <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>m</i></sub></span>. For each <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> he wants to know the expected height of the painted rectangle, provided that he selects <span class="tex-span"><i>x</i></span> for such fence uniformly among all <span class="tex-span"><i>n</i> - <i>k</i><sub class="lower-index"><i>i</i></sub> + 1</span> possible values. Help him to find the expected heights.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of planks in the fence. The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the height of the <span class="tex-span"><i>i</i></span>-th plank of the fence.</p><p>The third line contains an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> and the next line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> where <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is the width of the desired fuchsia-colored rectangle in planks.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> whitespace-separated real numbers, the <span class="tex-span"><i>i</i></span>-th number equals the expected value of the rectangle height, if its width in planks equals <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>. The value will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of planks in the fence. The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the height of the <span class="tex-span"><i>i</i></span>-th plank of the fence.</p><p>The third line contains an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> and the next line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> where <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is the width of the desired fuchsia-colored rectangle in planks.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> whitespace-separated real numbers, the <span class="tex-span"><i>i</i></span>-th number equals the expected value of the rectangle height, if its width in planks equals <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>. The value will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
3
3 2 1
3
1 2 3

```




```input2
2
1 1
3
1 2 1

```




```output1
2.000000000000000
1.500000000000000
1.000000000000000

```




```output2
1.000000000000000
1.000000000000000
1.000000000000000

```



## Note

<p>Let's consider the first sample test. </p><ul> <li> There are three possible positions of the fence for <span class="tex-span"><i>k</i><sub class="lower-index">1</sub> = 1</span>. For the first position <span class="tex-span">(<i>x</i> = 1)</span> the height is 3, for the second one <span class="tex-span">(<i>x</i> = 2)</span> the height is 2, for the third one <span class="tex-span">(<i>x</i> = 3)</span> the height is 1. As the fence position is chosen uniformly, the expected height of the fence equals <img align="middle" class="tex-formula" src="file://O5uYZrKD.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> There are two possible positions of the fence for <span class="tex-span"><i>k</i><sub class="lower-index">2</sub> = 2</span>. For the first position <span class="tex-span">(<i>x</i> = 1)</span> the height is 2, for the second one <span class="tex-span">(<i>x</i> = 2)</span> the height is 1. The expected height of the fence equals <img align="middle" class="tex-formula" src="file://Jflnl9vy.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> There is the only possible position of the fence for <span class="tex-span"><i>k</i><sub class="lower-index">3</sub> = 3</span>. The expected height of the fence equals 1. </li></ul>
