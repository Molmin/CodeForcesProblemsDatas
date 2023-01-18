## Description

<div><p><span class="tex-font-style-it">Rock... Paper!</span></p><p>After Karen have found the deterministic winning (losing?) strategy for rock-paper-scissors, her brother, Koyomi, comes up with a new game as a substitute. The game works as follows.</p><p>A positive integer <span class="tex-span"><i>n</i></span> is decided first. Both Koyomi and Karen independently choose <span class="tex-span"><i>n</i></span> distinct positive integers, denoted by <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> respectively. They reveal their sequences, and repeat until <span class="tex-font-style-bf">all of <span class="tex-span">2<i>n</i></span> integers become distinct</span>, which is the only final state to be kept and considered.</p><p>Then they count the number of ordered pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>) such that the value <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-tt">xor</span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span> equals to one of the <span class="tex-span">2<i>n</i></span> integers. Here <span class="tex-font-style-tt">xor</span> means the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise exclusive or</a> operation on two integers, and is denoted by operators <span class="tex-font-style-tt">^</span> and/or <span class="tex-font-style-tt">xor</span> in most programming languages.</p><p>Karen claims a win if the number of such pairs is even, and Koyomi does otherwise. And you're here to help determine the winner of their latest game.</p></div><div class="input-specification"><p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 000</span>) — the length of both sequences.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup></span>) — the integers finally chosen by Koyomi.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup></span>) — the integers finally chosen by Karen.</p><p>Input guarantees that <span class="tex-font-style-bf">the given <span class="tex-span">2<i>n</i></span> integers are pairwise distinct</span>, that is, no pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>) exists such that one of the following holds: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>; <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>j</i></sub></span>; <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>Output one line — the name of the winner, that is, "<span class="tex-font-style-tt">Koyomi</span>" or "<span class="tex-font-style-tt">Karen</span>" (without quotes). Please be aware of the capitalization.</p></div>

## Input

<p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 000</span>) — the length of both sequences.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup></span>) — the integers finally chosen by Koyomi.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup></span>) — the integers finally chosen by Karen.</p><p>Input guarantees that <span class="tex-font-style-bf">the given <span class="tex-span">2<i>n</i></span> integers are pairwise distinct</span>, that is, no pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>) exists such that one of the following holds: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>; <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>j</i></sub></span>; <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>.</p>

## Output

<p>Output one line — the name of the winner, that is, "<span class="tex-font-style-tt">Koyomi</span>" or "<span class="tex-font-style-tt">Karen</span>" (without quotes). Please be aware of the capitalization.</p>





```input1
3
1 2 3
4 5 6

```




```input2
5
2 4 6 8 10
9 7 5 3 1

```




```output1
Karen

```




```output2
Karen

```



## Note

<p>In the first example, there are <span class="tex-span">6</span> pairs satisfying the constraint: <span class="tex-span">(1, 1)</span>, <span class="tex-span">(1, 2)</span>, <span class="tex-span">(2, 1)</span>, <span class="tex-span">(2, 3)</span>, <span class="tex-span">(3, 2)</span> and <span class="tex-span">(3, 3)</span>. Thus, Karen wins since <span class="tex-span">6</span> is an even number.</p><p>In the second example, there are <span class="tex-span">16</span> such pairs, and Karen wins again.</p>
