## Description

<div><p>After waking up at <span class="tex-span"><i>hh</i></span>:<span class="tex-span"><i>mm</i></span>, Andrew realised that he had forgotten to feed his only cat for yet another time (guess why there's only one cat). The cat's current hunger level is <span class="tex-span"><i>H</i></span> points, moreover each minute without food increases his hunger by <span class="tex-span"><i>D</i></span> points.</p><p>At any time Andrew can visit the store where tasty buns are sold (you can assume that is doesn't take time to get to the store and back). One such bun costs <span class="tex-span"><i>C</i></span> roubles and decreases hunger by <span class="tex-span"><i>N</i></span> points. Since the demand for bakery drops heavily in the evening, there is a special <span class="tex-span">20%</span> discount for buns starting from <span class="tex-span">20</span>:<span class="tex-span">00</span> (note that the cost might become rational). Of course, buns cannot be sold by parts.</p><p>Determine the minimum amount of money Andrew has to spend in order to feed his cat. The cat is considered fed if its hunger level is less than or equal to zero.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>hh</i></span> and <span class="tex-span"><i>mm</i></span> <span class="tex-span">(00 ≤ <i>hh</i> ≤ 23, 00 ≤ <i>mm</i> ≤ 59)</span> — the time of Andrew's awakening.</p><p>The second line contains four integers <span class="tex-span"><i>H</i></span>, <span class="tex-span"><i>D</i></span>, <span class="tex-span"><i>C</i></span> and <span class="tex-span"><i>N</i></span> <span class="tex-span">(1 ≤ <i>H</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>D</i>, <i>C</i>, <i>N</i> ≤ 10<sup class="upper-index">2</sup>)</span>.</p></div><div class="output-specification"><p>Output the minimum amount of money to within three decimal digits. You answer is considered correct, if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://G18ggLsT.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>hh</i></span> and <span class="tex-span"><i>mm</i></span> <span class="tex-span">(00 ≤ <i>hh</i> ≤ 23, 00 ≤ <i>mm</i> ≤ 59)</span> — the time of Andrew's awakening.</p><p>The second line contains four integers <span class="tex-span"><i>H</i></span>, <span class="tex-span"><i>D</i></span>, <span class="tex-span"><i>C</i></span> and <span class="tex-span"><i>N</i></span> <span class="tex-span">(1 ≤ <i>H</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>D</i>, <i>C</i>, <i>N</i> ≤ 10<sup class="upper-index">2</sup>)</span>.</p>

## Output

<p>Output the minimum amount of money to within three decimal digits. You answer is considered correct, if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://G18ggLsT.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
19 00
255 1 100 1

```




```input2
17 41
1000 6 15 11

```




```output1
25200.0000

```




```output2
1365.0000

```



## Note

<p>In the first sample Andrew can visit the store at exactly <span class="tex-span">20</span>:<span class="tex-span">00</span>. The cat's hunger will be equal to <span class="tex-span">315</span>, hence it will be necessary to purchase <span class="tex-span">315</span> buns. The discount makes the final answer <span class="tex-span">25200</span> roubles.</p><p>In the second sample it's optimal to visit the store right after he wakes up. Then he'll have to buy <span class="tex-span">91</span> bins per <span class="tex-span">15</span> roubles each and spend a total of <span class="tex-span">1365</span> roubles.</p>
