## Description

<div><p><span class="tex-font-style-it">Pay attention: this problem is interactive.</span></p><p>Penguin Xoriy came up with a new game recently. He has <span class="tex-span"><i>n</i></span> icicles numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each icicle has a temperature&nbsp;— an integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>. <span class="tex-font-style-bf">Exactly two</span> of these icicles are special: their temperature is <span class="tex-span"><i>y</i></span>, while a temperature of all the others is <span class="tex-span"><i>x</i> ≠ <i>y</i></span>. You have to find those special icicles. You can choose a <span class="tex-font-style-it">non-empty</span> subset of icicles and ask the penguin what is the bitwise exclusive OR (<span class="tex-font-style-tt">XOR</span>) of the temperatures of the icicles in this subset. Note that you can't ask more than <span class="tex-font-style-bf">19</span> questions.</p><p>You are to find the special icicles.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i> ≠ <i>y</i></span>)&nbsp;— the number of icicles, the temperature of non-special icicles and the temperature of the special icicles.</p></div><div class="output-specification"><p>To give your answer to the penguin you have to print character "!" (without quotes), then print two integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub></span>)&nbsp;— the indexes of the special icicles <span class="tex-font-style-bf">in ascending order</span>. Note that "!" and <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> should be separated by a space; the indexes should be separated by a space too. After you gave the answer your program should terminate immediately.</p></div><div><h2>Interaction</h2><p>To ask a question print character "?" (without quotes), an integer <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ <i>n</i></span>), and <span class="tex-span"><i>c</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>p</i><sub class="lower-index"><i>c</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the indexes of icicles that you want to know about. Note that "?" and <span class="tex-span"><i>c</i></span> should be separated by a space; the indexes should be separated by a space too.</p><p>After you asked the question, read a single integer&nbsp;— the answer.</p><p>Note that you can't ask more than <span class="tex-font-style-bf">19</span> questions. If you ask more than 19 questions or at least one incorrect question, your solution will get "<span class="tex-font-style-tt">Wrong answer</span>".</p><p>If at some moment your program reads <span class="tex-span"> - 1</span> as an answer, it should immediately exit (for example, by calling exit(0)). You will get "<span class="tex-font-style-tt">Wrong answer</span>" in this case, it means that you asked more than 19 questions, or asked an invalid question. If you ignore this, you can get other verdicts since your program will continue to read from a closed stream.</p><p>Your solution will get "<span class="tex-font-style-tt">Idleness Limit Exceeded</span>", if you don't print anything or forget to flush the output, including for the final answer .</p><p>To flush you can use (just after printing): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> For other languages see the documentation. </li></ul><p><span class="tex-font-style-bf">Hacking</span></p><p>For hacking use the following format:</p><p><span class="tex-span"><i>n</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span></p><p>Here <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> ≤ <i>n</i></span> are the indexes of the special icicles.</p><p>Contestant programs will not be able to see this input.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i> ≠ <i>y</i></span>)&nbsp;— the number of icicles, the temperature of non-special icicles and the temperature of the special icicles.</p>

## Output

<p>To give your answer to the penguin you have to print character "!" (without quotes), then print two integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub></span>)&nbsp;— the indexes of the special icicles <span class="tex-font-style-bf">in ascending order</span>. Note that "!" and <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> should be separated by a space; the indexes should be separated by a space too. After you gave the answer your program should terminate immediately.</p>





```input1
4 2 1
2
1
1<span class="tex-font-style-it"></span>
```




```output1
? 3 1 2 3
? 1 1
? 1 3
! 1 3
```



## Note

<p>The answer for the first question is <img align="middle" class="tex-formula" src="file://jV6iWALu.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The answer for the second and the third questions is 1, therefore, special icicles are indexes 1 and 3.</p><p>You can read more about bitwise <span class="tex-font-style-tt">XOR</span> operation here: <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">https://en.wikipedia.org/wiki/Bitwise_operation#XOR</a>.</p>
