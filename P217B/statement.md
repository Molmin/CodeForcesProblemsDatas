## Description

<div><p>Fibonacci numbers are the sequence of integers: <span class="tex-span"><i>f</i><sub class="lower-index">0</sub> = 0</span>, <span class="tex-span"><i>f</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>f</i><sub class="lower-index">2</sub> = 1</span>, <span class="tex-span"><i>f</i><sub class="lower-index">3</sub> = 2</span>, <span class="tex-span"><i>f</i><sub class="lower-index">4</sub> = 3</span>, <span class="tex-span"><i>f</i><sub class="lower-index">5</sub> = 5</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i></sub> = <i>f</i><sub class="lower-index"><i>n</i> - 2</sub> + <i>f</i><sub class="lower-index"><i>n</i> - 1</sub></span>. So every next number is the sum of the previous two.</p><p>Bajtek has developed a nice way to compute Fibonacci numbers on a blackboard. First, he writes a 0. Then, below it, he writes a 1. Then he performs the following two operations:</p><ul> <li> operation "<span class="tex-font-style-tt">T</span>": replace the top number with the sum of both numbers; </li><li> operation "<span class="tex-font-style-tt">B</span>": replace the bottom number with the sum of both numbers. </li></ul><p>If he performs <span class="tex-span"><i>n</i></span> operations, starting with "<span class="tex-font-style-tt">T</span>" and then choosing operations alternately (so that the sequence of operations looks like "<span class="tex-font-style-tt">TBTBTBTB</span><span class="tex-span">...</span>"), the last number written will be equal to <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i> + 1</sub></span>.</p><p>Unfortunately, Bajtek sometimes makes mistakes and repeats an operation two or more times in a row. For example, if Bajtek wanted to compute <span class="tex-span"><i>f</i><sub class="lower-index">7</sub></span>, then he would want to do <span class="tex-span"><i>n</i> = 6</span> operations: "<span class="tex-font-style-tt">TBTBTB</span>". If he instead performs the sequence of operations "<span class="tex-font-style-tt">TTTBBT</span>", then he will have made 3 mistakes, and he will incorrectly compute that the seventh Fibonacci number is 10. The number of mistakes in the sequence of operations is the number of neighbouring equal operations («<span class="tex-font-style-tt">TT</span>» or «<span class="tex-font-style-tt">BB</span>»).</p><p>You are given the number <span class="tex-span"><i>n</i></span> of operations that Bajtek has made in an attempt to compute <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i> + 1</sub></span> and the number <span class="tex-span"><i>r</i></span> that is the result of his computations (that is last written number). Find the minimum possible number of mistakes that Bajtek must have made and any possible sequence of <span class="tex-span"><i>n</i></span> operations resulting in <span class="tex-span"><i>r</i></span> with that number of mistakes.</p><p>Assume that Bajtek always correctly starts with operation "<span class="tex-font-style-tt">T</span>".</p></div><div class="input-specification"><p>The first line contains the integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>r</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>The first line of the output should contain one number — the minimum possible number of mistakes made by Bajtek. The second line should contain <span class="tex-span"><i>n</i></span> characters, starting with "<span class="tex-font-style-tt">T</span>", describing one possible sequence of operations with that number of mistakes. Each character must be either "<span class="tex-font-style-tt">T</span>" or "<span class="tex-font-style-tt">B</span>".</p><p>If the required sequence doesn't exist, output "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without quotes).</p></div>

## Input

<p>The first line contains the integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>r</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>The first line of the output should contain one number — the minimum possible number of mistakes made by Bajtek. The second line should contain <span class="tex-span"><i>n</i></span> characters, starting with "<span class="tex-font-style-tt">T</span>", describing one possible sequence of operations with that number of mistakes. Each character must be either "<span class="tex-font-style-tt">T</span>" or "<span class="tex-font-style-tt">B</span>".</p><p>If the required sequence doesn't exist, output "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without quotes).</p>





```input1
6 10

```




```input2
4 5

```




```input3
2 1

```




```output1
2
TBBTTB

```




```output2
0
TBTB

```




```output3
IMPOSSIBLE

```


