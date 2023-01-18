## Description

<div><p>INTERCAL is the oldest of esoteric programming languages. One of its many weird features is the method of character-based output, known as Turing Tape method. It converts an array of unsigned 8-bit integers into a sequence of characters to print, using the following method.</p><p>The integers of the array are processed one by one, starting from the first. Processing <span class="tex-span"><i>i</i></span>-th element of the array is done in three steps:</p><p>1. The 8-bit binary notation of the ASCII-code of the previous printed character is reversed. When the first element of the array is processed, the result of this step is considered to be 0.</p><p>2. The <span class="tex-span"><i>i</i></span>-th element of the array is subtracted from the result of the previous step modulo 256.</p><p>3. The binary notation of the result of the previous step is reversed again to produce ASCII-code of the <span class="tex-span"><i>i</i></span>-th character to be printed.</p><p>You are given the text printed using this method. Restore the array used to produce this text.</p></div><div class="input-specification"><p>The input will consist of a single line <span class="tex-span"><i>text</i></span> which contains the message printed using the described method. String <span class="tex-span"><i>text</i></span> will contain between 1 and 100 characters, inclusive. ASCII-code of each character of <span class="tex-span"><i>text</i></span> will be between 32 (space) and 126 (tilde), inclusive.</p></div><div class="output-specification"><p>Output the initial array, which was used to produce <span class="tex-span"><i>text</i></span>, one integer per line.</p></div>

## Input

<p>The input will consist of a single line <span class="tex-span"><i>text</i></span> which contains the message printed using the described method. String <span class="tex-span"><i>text</i></span> will contain between 1 and 100 characters, inclusive. ASCII-code of each character of <span class="tex-span"><i>text</i></span> will be between 32 (space) and 126 (tilde), inclusive.</p>

## Output

<p>Output the initial array, which was used to produce <span class="tex-span"><i>text</i></span>, one integer per line.</p>





```input1
Hello, World!

```




```output1
238
108
112
0
64
194
48
26
244
168
24
16
162

```



## Note

<p>Let's have a closer look at the beginning of the example. The first character is "<span class="tex-font-style-tt">H</span>" with ASCII-code <span class="tex-span">72 = 01001000<sub class="lower-index">2</sub></span>. Its reverse is <span class="tex-span">00010010<sub class="lower-index">2</sub> = 18</span>, and this number should become the result of the second step of processing. The result of the first step is considered to be 0, so the first element of the array has to be <span class="tex-span">(0 - 18)</span> mod <span class="tex-span">256 = 238</span>, where <span class="tex-span"><i>a</i></span> mod <span class="tex-span"><i>b</i></span> is the remainder of division of <span class="tex-span"><i>a</i></span> by <span class="tex-span"><i>b</i></span>.</p>
