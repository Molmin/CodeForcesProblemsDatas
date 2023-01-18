## Description

<div><p>Unary is a minimalistic Brainfuck dialect in which programs are written using only one token. </p><p>Brainfuck programs use 8 commands: "<span class="tex-font-style-tt">+</span>", "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">[</span>", "<span class="tex-font-style-tt">]</span>", "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>", "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">,</span>" (their meaning is not important for the purposes of this problem). Unary programs are created from Brainfuck programs using the following algorithm. First, replace each command with a corresponding binary code, using the following conversion table: </p><ul> <li> "<span class="tex-font-style-tt">&gt;</span>" <span class="tex-span"> → </span> 1000, </li><li> "<span class="tex-font-style-tt">&lt;</span>" <span class="tex-span"> → </span> 1001, </li><li> "<span class="tex-font-style-tt">+</span>" <span class="tex-span"> → </span> 1010, </li><li> "<span class="tex-font-style-tt">-</span>" <span class="tex-span"> → </span> 1011, </li><li> "<span class="tex-font-style-tt">.</span>" <span class="tex-span"> → </span> 1100, </li><li> "<span class="tex-font-style-tt">,</span>" <span class="tex-span"> → </span> 1101, </li><li> "<span class="tex-font-style-tt">[</span>" <span class="tex-span"> → </span> 1110, </li><li> "<span class="tex-font-style-tt">]</span>" <span class="tex-span"> → </span> 1111. </li></ul><p>Next, concatenate the resulting binary codes into one binary number in the same order as in the program. Finally, write this number using unary numeral system — this is the Unary program equivalent to the original Brainfuck one.</p><p>You are given a Brainfuck program. Your task is to calculate the size of the equivalent Unary program, and print it modulo <span class="tex-span">1000003</span> <span class="tex-span">(10<sup class="upper-index">6</sup> + 3)</span>.</p></div><div class="input-specification"><p>The input will consist of a single line <span class="tex-span"><i>p</i></span> which gives a Brainfuck program. String <span class="tex-span"><i>p</i></span> will contain between 1 and 100 characters, inclusive. Each character of <span class="tex-span"><i>p</i></span> will be "<span class="tex-font-style-tt">+</span>", "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">[</span>", "<span class="tex-font-style-tt">]</span>", "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>", "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">,</span>".</p></div><div class="output-specification"><p>Output the size of the equivalent Unary program modulo <span class="tex-span">1000003</span> <span class="tex-span">(10<sup class="upper-index">6</sup> + 3)</span>.</p></div>

## Input

<p>The input will consist of a single line <span class="tex-span"><i>p</i></span> which gives a Brainfuck program. String <span class="tex-span"><i>p</i></span> will contain between 1 and 100 characters, inclusive. Each character of <span class="tex-span"><i>p</i></span> will be "<span class="tex-font-style-tt">+</span>", "<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">[</span>", "<span class="tex-font-style-tt">]</span>", "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>", "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">,</span>".</p>

## Output

<p>Output the size of the equivalent Unary program modulo <span class="tex-span">1000003</span> <span class="tex-span">(10<sup class="upper-index">6</sup> + 3)</span>.</p>





```input1
,.

```




```input2
++++[&gt;,.&lt;-]

```




```output1
220

```




```output2
61425

```



## Note

<p>To write a number <span class="tex-span"><i>n</i></span> in unary numeral system, one simply has to write 1 <span class="tex-span"><i>n</i></span> times. For example, 5 written in unary system will be 11111.</p><p>In the first example replacing Brainfuck commands with binary code will give us 1101 1100. After we concatenate the codes, we'll get 11011100 in binary system, or 220 in decimal. That's exactly the number of tokens in the equivalent Unary program.</p>
