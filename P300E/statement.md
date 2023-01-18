## Description

<div><p>In a far away galaxy there is war again. The treacherous Republic made <span class="tex-span"><i>k</i></span> precision strikes of power <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> on the Empire possessions. To cope with the republican threat, the Supreme Council decided to deal a decisive blow to the enemy forces. </p><p>To successfully complete the conflict, the confrontation balance after the blow should be a positive integer. The balance of confrontation is a number that looks like <img align="middle" class="tex-formula" src="file://pSXO1xhu.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>p</i> = <i>n</i>!</span> (<span class="tex-span"><i>n</i></span> is the power of the Imperial strike), <img align="middle" class="tex-formula" src="file://jaz287qi.png" style="max-width: 100.0%;max-height: 100.0%;">. After many years of war the Empire's resources are low. So to reduce the costs, <span class="tex-span"><i>n</i></span> should be a minimum positive integer that is approved by the commanders.</p><p>Help the Empire, find the minimum positive integer <span class="tex-span"><i>n</i></span>, where the described fraction is a positive integer.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span>.</p></div><div class="output-specification"><p>Print the minimum positive integer <span class="tex-span"><i>n</i></span>, needed for the Empire to win.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> to read or write 64-but integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span>.</p>

## Output

<p>Print the minimum positive integer <span class="tex-span"><i>n</i></span>, needed for the Empire to win.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> to read or write 64-but integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
2
1000 1000

```




```input2
1
2

```




```output1
2000
```




```output2
2
```


