## Description

<div><p>Recently Anton found a box with digits in his room. There are <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> digits <span class="tex-span">2</span>, <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span> digits <span class="tex-span">3</span>, <span class="tex-span"><i>k</i><sub class="lower-index">5</sub></span> digits <span class="tex-span">5</span> and <span class="tex-span"><i>k</i><sub class="lower-index">6</sub></span> digits <span class="tex-span">6</span>.</p><p>Anton's favorite integers are <span class="tex-span">32</span> and <span class="tex-span">256</span>. He decided to compose this integers from digits he has. He wants to make the sum of these integers as large as possible. Help him solve this task!</p><p>Each digit can be used no more than once, i.e. the composed integers should contain no more than <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> digits <span class="tex-span">2</span>, <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span> digits <span class="tex-span">3</span> and so on. Of course, unused digits are not counted in the sum.</p></div><div class="input-specification"><p>The only line of the input contains four integers <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">5</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">6</sub></span>&nbsp;— the number of digits <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span> respectively (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index">2</sub>, <i>k</i><sub class="lower-index">3</sub>, <i>k</i><sub class="lower-index">5</sub>, <i>k</i><sub class="lower-index">6</sub> ≤ 5·10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print one integer&nbsp;— maximum possible sum of Anton's favorite integers that can be composed using digits from the box.</p></div>

## Input

<p>The only line of the input contains four integers <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index">5</sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index">6</sub></span>&nbsp;— the number of digits <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span> respectively (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index">2</sub>, <i>k</i><sub class="lower-index">3</sub>, <i>k</i><sub class="lower-index">5</sub>, <i>k</i><sub class="lower-index">6</sub> ≤ 5·10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print one integer&nbsp;— maximum possible sum of Anton's favorite integers that can be composed using digits from the box.</p>





```input1
5 1 3 4

```




```input2
1 1 1 1

```




```output1
800

```




```output2
256

```



## Note

<p>In the first sample, there are five digits <span class="tex-span">2</span>, one digit <span class="tex-span">3</span>, three digits <span class="tex-span">5</span> and four digits <span class="tex-span">6</span>. Anton can compose three integers <span class="tex-span">256</span> and one integer <span class="tex-span">32</span> to achieve the value <span class="tex-span">256 + 256 + 256 + 32 = 800</span>. Note, that there is one unused integer <span class="tex-span">2</span> and one unused integer <span class="tex-span">6</span>. They are not counted in the answer.</p><p>In the second sample, the optimal answer is to create on integer <span class="tex-span">256</span>, thus the answer is <span class="tex-span">256</span>.</p>
