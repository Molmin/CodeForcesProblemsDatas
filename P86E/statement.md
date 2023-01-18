## Description

<div><p>A sequence <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ...</span> is called a <span class="tex-font-style-it">recurrent binary sequence</span>, if each term <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>i</i> = 0, 1, ...)</span> is equal to 0 or 1 and there exist coefficients <img align="middle" class="tex-formula" src="file://4EmOh22W.png" style="max-width: 100.0%;max-height: 100.0%;"> such that </p><center class="tex-equation"><span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = <i>c</i><sub class="lower-index">1</sub>·<i>a</i><sub class="lower-index"><i>n</i> - 1</sub> + <i>c</i><sub class="lower-index">2</sub>·<i>a</i><sub class="lower-index"><i>n</i> - 2</sub> + ... + <i>c</i><sub class="lower-index"><i>k</i></sub>·<i>a</i><sub class="lower-index"><i>n</i> - <i>k</i></sub> (<i>mod</i> 2), </span></center> for all <span class="tex-span"><i>n</i> ≥ <i>k</i></span>. Assume that not all of <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> are zeros.<p>Note that such a sequence can be uniquely recovered from any <span class="tex-span"><i>k</i></span>-tuple <span class="tex-span">{<i>a</i><sub class="lower-index"><i>s</i></sub>, <i>a</i><sub class="lower-index"><i>s</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>s</i> + <i>k</i> - 1</sub>}</span> and so it is periodic. Moreover, if a <span class="tex-span"><i>k</i></span>-tuple contains only zeros, then the sequence contains only zeros, so this case is not very interesting. Otherwise the minimal period of the sequence is not greater than <span class="tex-span">2<sup class="upper-index"><i>k</i></sup> - 1</span>, as <span class="tex-span"><i>k</i></span>-tuple determines next element, and there are <span class="tex-span">2<sup class="upper-index"><i>k</i></sup> - 1</span> non-zero <span class="tex-span"><i>k</i></span>-tuples. Let us call a sequence <span class="tex-font-style-it">long</span> if its minimal period is exactly <span class="tex-span">2<sup class="upper-index"><i>k</i></sup> - 1</span>. Your task is to find a long sequence for a given <span class="tex-span"><i>k</i></span>, if there is any.</p></div><div class="input-specification"><p>Input contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 50</span>).</p></div><div class="output-specification"><p>If there is no long sequence for a given <span class="tex-span"><i>k</i></span>, output "-1" (without quotes). Otherwise the first line of the output should contain <span class="tex-span"><i>k</i></span> integer numbers: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> (coefficients). The second line should contain first <span class="tex-span"><i>k</i></span> elements of the sequence: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i> - 1</sub></span>. All of them (elements and coefficients) should be equal to 0 or 1, and at least one <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> has to be equal to 1.</p><p>If there are several solutions, output any.</p></div>

## Input

<p>Input contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 50</span>).</p>

## Output

<p>If there is no long sequence for a given <span class="tex-span"><i>k</i></span>, output "-1" (without quotes). Otherwise the first line of the output should contain <span class="tex-span"><i>k</i></span> integer numbers: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> (coefficients). The second line should contain first <span class="tex-span"><i>k</i></span> elements of the sequence: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i> - 1</sub></span>. All of them (elements and coefficients) should be equal to 0 or 1, and at least one <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> has to be equal to 1.</p><p>If there are several solutions, output any.</p>





```input1
2

```




```input2
3

```




```output1
1 1
1 0

```




```output2
0 1 1
1 1 1

```



## Note

<p>1. In the first sample: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub> = 1</span>, so <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = <i>a</i><sub class="lower-index"><i>n</i> - 1</sub> + <i>a</i><sub class="lower-index"><i>n</i> - 2</sub>  (<i>mod</i> 2)</span>. Thus the sequence will be:</p><center><img class="tex-graphics" src="file://rkOEU55T.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>so its period equals <span class="tex-span">3 = 2<sup class="upper-index">2</sup> - 1</span>.</p><p>2. In the second sample: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub> = 1</span>, <span class="tex-span"><i>c</i><sub class="lower-index">3</sub> = 1</span>, so <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = <i>a</i><sub class="lower-index"><i>n</i> - 2</sub> + <i>a</i><sub class="lower-index"><i>n</i> - 3</sub>  (<i>mod</i> 2)</span>. Thus our sequence is:</p><center><img class="tex-graphics" src="file://Ty3j5H4T.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>and its period equals <span class="tex-span">7 = 2<sup class="upper-index">3</sup> - 1</span>.</p><p>Periods are colored.</p>
