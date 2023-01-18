## Description

<div><p>Xenia has a set of weights and pan scales. Each weight has an integer weight from 1 to 10 kilos. Xenia is going to play with scales and weights a little. For this, she puts weights on the scalepans, one by one. The first weight goes on the left scalepan, the second weight goes on the right scalepan, the third one goes on the left scalepan, the fourth one goes on the right scalepan and so on. Xenia wants to put the total of <span class="tex-span"><i>m</i></span> weights on the scalepans.</p><p>Simply putting weights on the scales is not interesting, so Xenia has set some rules. First, she does not put on the scales two consecutive weights of the same weight. That is, the weight that goes <span class="tex-span"><i>i</i></span>-th should be different from the <span class="tex-span">(<i>i</i> + 1)</span>-th weight for any <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>m</i>)</span>. Second, every time Xenia puts a weight on some scalepan, she wants this scalepan to outweigh the other one. That is, the sum of the weights on the corresponding scalepan must be strictly greater than the sum on the other pan.</p><p>You are given all types of weights available for Xenia. You can assume that the girl has an infinite number of weights of each specified type. Your task is to help Xenia lay <span class="tex-span"><i>m</i></span> weights on ​​the scales or to say that it can't be done.</p></div><div class="input-specification"><p>The first line contains a string consisting of exactly ten zeroes and ones: the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(<i>i</i> ≥ 1)</span> character in the line equals "<span class="tex-font-style-tt">1</span>" if Xenia has <span class="tex-span"><i>i</i></span> kilo weights, otherwise the character equals "<span class="tex-font-style-tt">0</span>". The second line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 1000)</span>.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>", if there is a way to put <span class="tex-span"><i>m</i></span> weights on the scales by all rules. Otherwise, print in the first line "<span class="tex-font-style-tt">NO</span>". If you can put <span class="tex-span"><i>m</i></span> weights on the scales, then print in the next line <span class="tex-span"><i>m</i></span> integers — the weights' weights in the order you put them on the scales.</p><p>If there are multiple solutions, you can print any of them.</p></div>

## Input

<p>The first line contains a string consisting of exactly ten zeroes and ones: the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(<i>i</i> ≥ 1)</span> character in the line equals "<span class="tex-font-style-tt">1</span>" if Xenia has <span class="tex-span"><i>i</i></span> kilo weights, otherwise the character equals "<span class="tex-font-style-tt">0</span>". The second line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 1000)</span>.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>", if there is a way to put <span class="tex-span"><i>m</i></span> weights on the scales by all rules. Otherwise, print in the first line "<span class="tex-font-style-tt">NO</span>". If you can put <span class="tex-span"><i>m</i></span> weights on the scales, then print in the next line <span class="tex-span"><i>m</i></span> integers — the weights' weights in the order you put them on the scales.</p><p>If there are multiple solutions, you can print any of them.</p>





```input1
0000000101
3

```




```input2
1000000000
2

```




```output1
YES
8 10 8

```




```output2
NO

```


