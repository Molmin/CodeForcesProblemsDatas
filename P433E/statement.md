## Description

<div><p>Tachibana Kanade likes Mapo Tofu very much. One day, the canteen cooked all kinds of tofu to sell, but not all tofu is Mapo Tofu, only those spicy enough can be called Mapo Tofu.</p><p>Each piece of tofu in the canteen is given a <span class="tex-span"><i>m</i></span>-based number, all numbers are in the range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> (<span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> being <span class="tex-span"><i>m</i></span>-based numbers), and for every <span class="tex-span"><i>m</i></span>-based integer in the range <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, there exists a piece of tofu with that number.</p><p>To judge what tofu is Mapo Tofu, Tachibana Kanade chose <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>m</i></span>-based number strings, and assigned a value to each string. If a string appears in the number of a tofu, the value of the string will be added to the value of that tofu. If a string appears multiple times, then the value is also added that many times. Initially the value of each tofu is zero.</p><p>Tachibana Kanade considers tofu with values no more than <span class="tex-span"><i>k</i></span> to be Mapo Tofu. So now Tachibana Kanade wants to know, how many pieces of tofu are Mapo Tofu?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i>&nbsp;(1 ≤ <i>n</i> ≤ 200;&nbsp;2 ≤ <i>m</i> ≤ 20;&nbsp;1 ≤ <i>k</i> ≤ 500)</span>. Where <span class="tex-span"><i>n</i></span> denotes the number of strings, <span class="tex-span"><i>m</i></span> denotes the base used, and <span class="tex-span"><i>k</i></span> denotes the limit of the value for Mapo Tofu.</p><p>The second line represents the number <span class="tex-span"><i>l</i></span>. The first integer in the line is <span class="tex-span"><i>len</i></span> <span class="tex-span">(1 ≤ <i>len</i> ≤ 200)</span>, describing the length (number of digits in base <span class="tex-span"><i>m</i></span>) of <span class="tex-span"><i>l</i></span>. Then follow <span class="tex-span"><i>len</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>len</i></sub>&nbsp;(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>m</i>;&nbsp;<i>a</i><sub class="lower-index">1</sub> &gt; 0)</span> separated by spaces, representing the digits of <span class="tex-span"><i>l</i></span>, with <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> being the highest digit and <span class="tex-span"><i>a</i><sub class="lower-index"><i>len</i></sub></span> being the lowest digit.</p><p>The third line represents the number <span class="tex-span"><i>r</i></span> in the same format as <span class="tex-span"><i>l</i></span>. It is guaranteed that <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i></span>.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each line describing a number string. The <span class="tex-span"><i>i</i></span>-th line contains the <span class="tex-span"><i>i</i></span>-th number string and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> — the value of the <span class="tex-span"><i>i</i></span>-th string (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>). All number strings are described in almost the same format as <span class="tex-span"><i>l</i></span>, the only difference is number strings may contain necessary leading zeros (see the first example). The sum of the lengths of all number strings does not exceed <span class="tex-span">200</span>.</p></div><div class="output-specification"><p>Output the number of pieces of Mapo Tofu modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. The answer should be a decimal integer.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i>&nbsp;(1 ≤ <i>n</i> ≤ 200;&nbsp;2 ≤ <i>m</i> ≤ 20;&nbsp;1 ≤ <i>k</i> ≤ 500)</span>. Where <span class="tex-span"><i>n</i></span> denotes the number of strings, <span class="tex-span"><i>m</i></span> denotes the base used, and <span class="tex-span"><i>k</i></span> denotes the limit of the value for Mapo Tofu.</p><p>The second line represents the number <span class="tex-span"><i>l</i></span>. The first integer in the line is <span class="tex-span"><i>len</i></span> <span class="tex-span">(1 ≤ <i>len</i> ≤ 200)</span>, describing the length (number of digits in base <span class="tex-span"><i>m</i></span>) of <span class="tex-span"><i>l</i></span>. Then follow <span class="tex-span"><i>len</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>len</i></sub>&nbsp;(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>m</i>;&nbsp;<i>a</i><sub class="lower-index">1</sub> &gt; 0)</span> separated by spaces, representing the digits of <span class="tex-span"><i>l</i></span>, with <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> being the highest digit and <span class="tex-span"><i>a</i><sub class="lower-index"><i>len</i></sub></span> being the lowest digit.</p><p>The third line represents the number <span class="tex-span"><i>r</i></span> in the same format as <span class="tex-span"><i>l</i></span>. It is guaranteed that <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i></span>.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each line describing a number string. The <span class="tex-span"><i>i</i></span>-th line contains the <span class="tex-span"><i>i</i></span>-th number string and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> — the value of the <span class="tex-span"><i>i</i></span>-th string (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>). All number strings are described in almost the same format as <span class="tex-span"><i>l</i></span>, the only difference is number strings may contain necessary leading zeros (see the first example). The sum of the lengths of all number strings does not exceed <span class="tex-span">200</span>.</p>

## Output

<p>Output the number of pieces of Mapo Tofu modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. The answer should be a decimal integer.</p>





```input1
2 10 1
1 1
3 1 0 0
1 1 1
1 0 1

```




```input2
2 10 12
2 5 9
6 6 3 5 4 9 7
2 0 6 1
3 6 7 2 1

```




```input3
4 2 6
6 1 0 1 1 1 0
6 1 1 0 1 0 0
1 1 2
3 0 1 0 5
4 0 1 1 0 4
3 1 0 1 2

```




```output1
97

```




```output2
635439

```




```output3
2

```



## Note

<p>In the first sample, 10, 11 and 100 are the only three decimal numbers in <span class="tex-span">[1, 100]</span> with a value greater than 1. Here the value of 1 is 1 but not 2, since numbers cannot contain leading zeros and thus cannot be written as "<span class="tex-font-style-tt">01</span>".</p><p>In the second sample, no numbers in the given interval have a value greater than 12.</p><p>In the third sample, 110000 and 110001 are the only two binary numbers in the given interval with a value no greater than 6.</p>
