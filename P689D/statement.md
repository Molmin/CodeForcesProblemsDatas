## Description

<div><p>Mike and !Mike are old childhood rivals, they are opposite in everything they do, except programming. Today they have a problem they cannot solve on their own, but together (with you)&nbsp;— who knows? </p><p>Every one of them has an integer sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>n</i></span>. Being given a query of the form of pair of integers <span class="tex-span">(<i>l</i>, <i>r</i>)</span>, Mike can instantly tell the value of <img align="middle" class="tex-formula" src="file://w0htF51w.png" style="max-width: 100.0%;max-height: 100.0%;"> while !Mike can instantly tell the value of <img align="middle" class="tex-formula" src="file://AgNoY9rw.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Now suppose a robot (you!) asks them all possible different queries of pairs of integers <span class="tex-span">(<i>l</i>, <i>r</i>)</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span> (so he will make exactly <span class="tex-span"><i>n</i>(<i>n</i> + 1) / 2</span> queries) and counts how many times their answers coincide, thus for how many pairs <img align="middle" class="tex-formula" src="file://kJuJHQan.png" style="max-width: 100.0%;max-height: 100.0%;"> is satisfied.</p><p>How many occasions will the robot count?</p></div><div class="input-specification"><p>The first line contains only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the sequence <span class="tex-span"><i>a</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the sequence <span class="tex-span"><i>b</i></span>.</p></div><div class="output-specification"><p>Print the only integer number&nbsp;— the number of occasions the robot will count, thus for how many pairs <img align="middle" class="tex-formula" src="file://J28S7TBq.png" style="max-width: 100.0%;max-height: 100.0%;"> is satisfied.</p></div>

## Input

<p>The first line contains only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the sequence <span class="tex-span"><i>a</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the sequence <span class="tex-span"><i>b</i></span>.</p>

## Output

<p>Print the only integer number&nbsp;— the number of occasions the robot will count, thus for how many pairs <img align="middle" class="tex-formula" src="file://J28S7TBq.png" style="max-width: 100.0%;max-height: 100.0%;"> is satisfied.</p>





```input1
6
1 2 3 2 1 4
6 7 1 2 3 2

```




```input2
3
3 3 3
1 1 1

```




```output1
2

```




```output2
0

```



## Note

<p>The occasions in the first sample case are:</p><p>1.<span class="tex-span"><i>l</i> = 4</span>,<span class="tex-span"><i>r</i> = 4</span> since <span class="tex-span"><i>max</i>{2} = <i>min</i>{2}</span>.</p><p>2.<span class="tex-span"><i>l</i> = 4</span>,<span class="tex-span"><i>r</i> = 5</span> since <span class="tex-span"><i>max</i>{2, 1} = <i>min</i>{2, 3}</span>.</p><p>There are no occasions in the second sample case since Mike will answer <span class="tex-span">3</span> to any query pair, but !Mike will always answer <span class="tex-span">1</span>.</p>
