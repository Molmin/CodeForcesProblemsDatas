## Description

<div><p>Petya learned a new programming language CALPAS. A program in this language always takes one non-negative integer and returns one non-negative integer as well.</p><p>In the language, there are only three commands: apply a bitwise operation AND, OR or XOR with a given constant to the current integer. A program can contain an arbitrary sequence of these operations with arbitrary constants from <span class="tex-span">0</span> to <span class="tex-span">1023</span>. When the program is run, all operations are applied (in the given order) to the argument and in the end the result integer is returned.</p><p>Petya wrote a program in this language, but it turned out to be too long. Write a program in CALPAS that does the same thing as the Petya's program, and consists of no more than <span class="tex-span">5</span> lines. Your program should return the same integer as Petya's program for all arguments from <span class="tex-span">0</span> to <span class="tex-span">1023</span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of lines.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain commands. A command consists of a character that represents the operation ("<span class="tex-font-style-tt">&amp;</span>", "<span class="tex-font-style-tt">|</span>" or "<span class="tex-font-style-tt">^</span>" for AND, OR or XOR respectively), and the constant <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1023</span>.</p></div><div class="output-specification"><p>Output an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 5</span>) — the length of your program.</p><p>Next <span class="tex-span"><i>k</i></span> lines must contain commands in the same format as in the input.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of lines.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain commands. A command consists of a character that represents the operation ("<span class="tex-font-style-tt">&amp;</span>", "<span class="tex-font-style-tt">|</span>" or "<span class="tex-font-style-tt">^</span>" for AND, OR or XOR respectively), and the constant <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1023</span>.</p>

## Output

<p>Output an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 5</span>) — the length of your program.</p><p>Next <span class="tex-span"><i>k</i></span> lines must contain commands in the same format as in the input.</p>





```input1
3
| 3
^ 2
| 1

```




```input2
3
&amp; 1
&amp; 3
&amp; 5

```




```input3
3
^ 1
^ 2
^ 3

```




```output1
2
| 3
^ 2

```




```output2
1
&amp; 1

```




```output3
0

```



## Note

<p>You can read about bitwise operations in <a href="https://en.wikipedia.org/wiki/Bitwise_operation">https://en.wikipedia.org/wiki/Bitwise_operation</a>.</p><p>Second sample:</p><p>Let <span class="tex-span"><i>x</i></span> be an input of the Petya's program. It's output is <span class="tex-span">((<i>x</i>&amp;1)&amp;3)&amp;5 = <i>x</i>&amp;(1&amp;3&amp;5) = <i>x</i>&amp;1</span>. So these two programs always give the same outputs.</p>
