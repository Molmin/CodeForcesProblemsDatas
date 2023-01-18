## Description

<div><p>Roma (a popular Russian name that means 'Roman') loves the Little Lvov Elephant's lucky numbers.</p><p>Let us remind you that lucky numbers are positive integers whose decimal representation only contains lucky digits <span class="tex-span">4</span> and <span class="tex-span">7</span>. For example, numbers <span class="tex-span">47</span>, <span class="tex-span">744</span>, <span class="tex-span">4</span> are lucky and <span class="tex-span">5</span>, <span class="tex-span">17</span>, <span class="tex-span">467</span> are not.</p><p>Roma's got <span class="tex-span"><i>n</i></span> positive integers. He wonders, how many of those integers have not more than <span class="tex-span"><i>k</i></span> lucky digits? Help him, write the program that solves the problem.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the numbers that Roma has. </p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 100)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the numbers that Roma has. </p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>In a single line print a single integer — the answer to the problem.</p>





```input1
3 4
1 2 4

```




```input2
3 2
447 44 77

```




```output1
3

```




```output2
2

```



## Note

<p>In the first sample all numbers contain at most four lucky digits, so the answer is <span class="tex-span">3</span>.</p><p>In the second sample number <span class="tex-span">447</span> doesn't fit in, as it contains more than two lucky digits. All other numbers are fine, so the answer is <span class="tex-span">2</span>.</p>
