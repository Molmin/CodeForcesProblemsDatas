## Description

<div><p>Vasya should paint a fence in front of his own cottage. The fence is a sequence of <span class="tex-span"><i>n</i></span> wooden boards arranged in a single row. Each board is a <span class="tex-span">1</span> centimeter wide rectangle. Let's number the board fence using numbers <span class="tex-span">1, 2, ..., <i>n</i></span> from left to right. The height of the <span class="tex-span"><i>i</i></span>-th board is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> centimeters.</p><p>Vasya has a <span class="tex-span">1</span> centimeter wide brush and the paint of two colors, red and green. Of course, the amount of the paint is limited. Vasya counted the area he can paint each of the colors. It turned out that he can not paint over <span class="tex-span"><i>a</i></span> square centimeters of the fence red, and he can not paint over <span class="tex-span"><i>b</i></span> square centimeters green. Each board of the fence should be painted exactly one of the two colors. Perhaps Vasya won't need one of the colors.</p><p>In addition, Vasya wants his fence to look smart. To do this, he should paint the fence so as to minimize the value that Vasya called the fence <span class="tex-font-style-it">unattractiveness</span> value. Vasya believes that two consecutive fence boards, painted different colors, look unattractive. The <span class="tex-font-style-it">unattractiveness</span> value of a fence is the total length of contact between the neighboring boards of various colors. To make the fence look nice, you need to minimize the value as low as possible. Your task is to find what is the minimum unattractiveness Vasya can get, if he paints his fence completely.</p><center> <img class="tex-graphics" src="file://1F6PXSWn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The picture shows the fence, where the heights of boards (from left to right) are 2,3,2,4,3,1. The first and the fifth boards are painted red, the others are painted green. The first and the second boards have contact length 2, the fourth and fifth boards have contact length 3, the fifth and the sixth have contact length 1. Therefore, the <span class="tex-font-style-it">unattractiveness</span> of the given painted fence is 2+3+1=6.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the number of boards in Vasya's fence.</p><p>The second line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 4·10<sup class="upper-index">4</sup></span>) — the area that can be painted red and the area that can be painted green, correspondingly.</p><p>The third line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 200)</span> — the heights of the fence boards.</p><p>All numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print a single number — the minimum <span class="tex-font-style-it">unattractiveness</span> value Vasya can get if he paints his fence completely. If it is impossible to do, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the number of boards in Vasya's fence.</p><p>The second line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 4·10<sup class="upper-index">4</sup></span>) — the area that can be painted red and the area that can be painted green, correspondingly.</p><p>The third line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 200)</span> — the heights of the fence boards.</p><p>All numbers in the lines are separated by single spaces.</p>

## Output

<p>Print a single number — the minimum <span class="tex-font-style-it">unattractiveness</span> value Vasya can get if he paints his fence completely. If it is impossible to do, print <span class="tex-span"> - 1</span>.</p>





```input1
4
5 7
3 3 4 1

```




```input2
3
2 3
1 3 1

```




```input3
3
3 3
2 2 2

```




```output1
3

```




```output2
2

```




```output3
-1

```


