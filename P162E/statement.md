## Description

<div><p>HQ9+ is a joke programming language which has only four one-character instructions:</p><ul><li> "<span class="tex-font-style-tt">H</span>" prints "<span class="tex-font-style-tt">Hello, World!</span>",</li><li> "<span class="tex-font-style-tt">Q</span>" prints the whole source code of the program itself (at each call),</li><li> "<span class="tex-font-style-tt">9</span>" prints the lyrics of "99 Bottles of Beer" song, </li><li> "<span class="tex-font-style-tt">+</span>" increments the value stored in the internal accumulator.</li></ul><p>Instructions "<span class="tex-font-style-tt">H</span>" and "<span class="tex-font-style-tt">Q</span>" are case-sensitive and must be uppercase. The characters of the program which are not instructions are ignored.</p><p>You are given a program written in HQ9+. You have to figure out whether executing this program will produce any output.</p></div><div class="input-specification"><p>The input will consist of a single line <span class="tex-span"><i>p</i></span> which will give a program in HQ9+. String <span class="tex-span"><i>p</i></span> will contain between 1 and 100 characters, inclusive. ASCII-code of each character of <span class="tex-span"><i>p</i></span> will be between 33 (exclamation mark) and 126 (tilde), inclusive.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>", if executing the program will produce any output, and "<span class="tex-font-style-tt">NO</span>" otherwise (quotes for clarity only).</p></div>

## Input

<p>The input will consist of a single line <span class="tex-span"><i>p</i></span> which will give a program in HQ9+. String <span class="tex-span"><i>p</i></span> will contain between 1 and 100 characters, inclusive. ASCII-code of each character of <span class="tex-span"><i>p</i></span> will be between 33 (exclamation mark) and 126 (tilde), inclusive.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>", if executing the program will produce any output, and "<span class="tex-font-style-tt">NO</span>" otherwise (quotes for clarity only).</p>





```input1
Hello!

```




```input2
VK_Cup_2012!

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first case the program contains only one instruction — "<span class="tex-font-style-tt">H</span>", which prints "<span class="tex-font-style-tt">Hello, World!</span>".</p><p>In the second case none of the program characters are language instructions.</p>
