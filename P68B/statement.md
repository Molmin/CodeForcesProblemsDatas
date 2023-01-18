## Description

<div><p>It is well known that the planet suffers from the energy crisis. Little Petya doesn't like that and wants to save the world. For this purpose he needs every accumulator to contain the same amount of energy. Initially every accumulator has some amount of energy: the <span class="tex-span"><i>i</i></span>-th accumulator has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> units of energy. Energy can be transferred from one accumulator to the other. Every time <span class="tex-span"><i>x</i></span> units of energy are transferred (<span class="tex-span"><i>x</i></span> is not necessarily an integer) <span class="tex-span"><i>k</i></span> percent of it is lost. That is, if <span class="tex-span"><i>x</i></span> units were transferred from one accumulator to the other, amount of energy in the first one decreased by <span class="tex-span"><i>x</i></span> units and in other increased by <img align="middle" class="tex-formula" src="file://yvCElXLj.png" style="max-width: 100.0%;max-height: 100.0%;"> units.</p><p>Your task is to help Petya find what maximum equal amount of energy can be stored in each accumulator after the transfers.</p></div><div class="input-specification"><p>First line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000, 0 ≤ <i>k</i> ≤ 99</span>) — number of accumulators and the percent of energy that is lost during transfers.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> — amounts of energy in the first, second, .., <span class="tex-span"><i>n</i></span>-th accumulator respectively (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, 1 ≤ <i>i</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Output maximum possible amount of energy that can remain in each of accumulators after the transfers of energy.</p><p>The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>First line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000, 0 ≤ <i>k</i> ≤ 99</span>) — number of accumulators and the percent of energy that is lost during transfers.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> — amounts of energy in the first, second, .., <span class="tex-span"><i>n</i></span>-th accumulator respectively (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, 1 ≤ <i>i</i> ≤ <i>n</i></span>).</p>

## Output

<p>Output maximum possible amount of energy that can remain in each of accumulators after the transfers of energy.</p><p>The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3 50
4 2 1

```




```input2
2 90
1 11

```




```output1
2.000000000

```




```output2
1.909090909

```


