## Description

<div><p>There are <span class="tex-span"><i>n</i></span> piles of pebbles on the table, the <span class="tex-span"><i>i</i></span>-th pile contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> pebbles. Your task is to paint each pebble using one of the <span class="tex-span"><i>k</i></span> given colors so that for each color <span class="tex-span"><i>c</i></span> and any two piles <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> the difference between the number of pebbles of color <span class="tex-span"><i>c</i></span> in pile <span class="tex-span"><i>i</i></span> and number of pebbles of color <span class="tex-span"><i>c</i></span> in pile <span class="tex-span"><i>j</i></span> is at most one.</p><p>In other words, let's say that <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, <i>c</i></sub></span> is the number of pebbles of color <span class="tex-span"><i>c</i></span> in the <span class="tex-span"><i>i</i></span>-th pile. Then for any <span class="tex-span">1 ≤ <i>c</i> ≤ <i>k</i></span>, <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span> the following condition must be satisfied <span class="tex-span">|<i>b</i><sub class="lower-index"><i>i</i>, <i>c</i></sub> - <i>b</i><sub class="lower-index"><i>j</i>, <i>c</i></sub>| ≤ 1</span>. It isn't necessary to use all <span class="tex-span"><i>k</i></span> colors: if color <span class="tex-span"><i>c</i></span> hasn't been used in pile <span class="tex-span"><i>i</i></span>, then <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, <i>c</i></sub></span> is considered to be zero.</p></div><div class="input-specification"><p>The first line of the input contains positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>), separated by a space — the number of piles and the number of colors respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) denoting number of pebbles in each of the piles.</p></div><div class="output-specification"><p>If there is no way to paint the pebbles satisfying the given condition, output "<span class="tex-font-style-tt">NO</span>" (without quotes) .</p><p>Otherwise in the first line output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then <span class="tex-span"><i>n</i></span> lines should follow, the <span class="tex-span"><i>i</i></span>-th of them should contain <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers. <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>) of these integers should be equal to the color of the <span class="tex-span"><i>j</i></span>-th pebble in the <span class="tex-span"><i>i</i></span>-th pile. <span class="tex-font-style-bf">If there are several possible answers, you may output any of them.</span></p></div>

## Input

<p>The first line of the input contains positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>), separated by a space — the number of piles and the number of colors respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) denoting number of pebbles in each of the piles.</p>

## Output

<p>If there is no way to paint the pebbles satisfying the given condition, output "<span class="tex-font-style-tt">NO</span>" (without quotes) .</p><p>Otherwise in the first line output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then <span class="tex-span"><i>n</i></span> lines should follow, the <span class="tex-span"><i>i</i></span>-th of them should contain <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers. <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>) of these integers should be equal to the color of the <span class="tex-span"><i>j</i></span>-th pebble in the <span class="tex-span"><i>i</i></span>-th pile. <span class="tex-font-style-bf">If there are several possible answers, you may output any of them.</span></p>





```input1
4 4
1 2 3 4

```




```input2
5 2
3 2 4 1 3

```




```input3
5 4
3 2 4 3 5

```




```output1
YES
1
1 4
1 2 4
1 2 3 4

```




```output2
NO

```




```output3
YES
1 2 3
1 3
1 2 3 4
1 3 4
1 1 2 3 4

```


