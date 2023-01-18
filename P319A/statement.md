## Description

<div><p>As a tradition, every year before IOI all the members of Natalia Fan Club are invited to Malek Dance Club to have a fun night together. Malek Dance Club has <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> members and coincidentally Natalia Fan Club also has <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> members. Each member of MDC is assigned a unique id <span class="tex-span"><i>i</i></span> from <span class="tex-span">0</span> to <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> - 1</span>. The same holds for each member of NFC.</p><p>One of the parts of this tradition is one by one dance, where each member of MDC dances with a member of NFC. A dance pair is a pair of numbers <span class="tex-span">(<i>a</i>, <i>b</i>)</span> such that member <span class="tex-span"><i>a</i></span> from MDC dances with member <span class="tex-span"><i>b</i></span> from NFC.</p><p>The complexity of a pairs' assignment is the number of pairs of dancing pairs <span class="tex-span">(<i>a</i>, <i>b</i>)</span> and <span class="tex-span">(<i>c</i>, <i>d</i>)</span> such that <span class="tex-span"><i>a</i> &lt; <i>c</i></span> and <span class="tex-span"><i>b</i> &gt; <i>d</i></span>.</p><p>You are given a binary number of length <span class="tex-span"><i>n</i></span> named <span class="tex-span"><i>x</i></span>. We know that member <span class="tex-span"><i>i</i></span> from MDC dances with member <img align="middle" class="tex-formula" src="file://dmHtKHja.png" style="max-width: 100.0%;max-height: 100.0%;"> from NFC. Your task is to calculate the complexity of this assignment modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>Expression <img align="middle" class="tex-formula" src="file://0CSRdays.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes applying «XOR» to numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. This operation exists in all modern programming languages, for example, in <span class="tex-font-style-it">C++</span> and <span class="tex-font-style-it">Java</span> it denotes as «<span class="tex-font-style-tt">^</span>», in <span class="tex-font-style-it">Pascal</span> — «<span class="tex-font-style-tt">xor</span>».</p></div><div class="input-specification"><p>The first line of input contains a binary number <span class="tex-span"><i>x</i></span> of lenght <span class="tex-span"><i>n</i></span>, <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>.</p><p>This number may contain leading zeros.</p></div><div class="output-specification"><p>Print the complexity of the given dance assignent modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line of input contains a binary number <span class="tex-span"><i>x</i></span> of lenght <span class="tex-span"><i>n</i></span>, <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span>.</p><p>This number may contain leading zeros.</p>

## Output

<p>Print the complexity of the given dance assignent modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
11

```




```input2
01

```




```input3
1

```




```output1
6

```




```output2
2

```




```output3
1

```


