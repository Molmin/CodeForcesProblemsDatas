## Description

<div><p>Borya has recently found a big electronic display. The computer that manages the display stores some integer number. The number has <span class="tex-span"><i>n</i></span> decimal digits, the display shows the encoded version of the number, where each digit is shown using some lowercase letter of the English alphabet.</p><p>There is a legend near the display, that describes how the number is encoded. For each digit position <span class="tex-span"><i>i</i></span> and each digit <span class="tex-span"><i>j</i></span> the character <span class="tex-span"><i>c</i></span> is known, that encodes this digit at this position. Different digits can have the same code characters.</p><p>Each second the number is increased by 1. And one second after a moment when the number reaches the value that is represented as <span class="tex-span"><i>n</i></span> 9-s in decimal notation, the loud beep sounds. </p><p>Andrew knows the number that is stored in the computer. Now he wants to know how many seconds must pass until Borya can definitely tell what was the original number encoded by the display. Assume that Borya can precisely measure time, and that the encoded number will first be increased exactly one second after Borya started watching at the display.</p></div><div class="input-specification"><p>Input data contains multiple test cases. The first line of input contains <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>)&nbsp;— the number of test cases. </p><p>Each test case is described as follows. The first line of the description contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>)&nbsp;— the number of digits in the number. The second line contains <span class="tex-span"><i>n</i></span> decimal digits without spaces (but possibly with leading zeroes)&nbsp;— the number initially stored in the display computer. The following <span class="tex-span"><i>n</i></span> lines contain 10 characters each. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th of these lines is the code character for a digit <span class="tex-span"><i>j</i> - 1</span> in position <span class="tex-span"><i>i</i></span>, most significant digit positions are described first.</p></div><div class="output-specification"><p>For each test case print an integer: the number of seconds until Borya definitely knows what was the initial number stored on the display of the computer. Do not print leading zeroes.</p></div>

## Input

<p>Input data contains multiple test cases. The first line of input contains <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>)&nbsp;— the number of test cases. </p><p>Each test case is described as follows. The first line of the description contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 18</span>)&nbsp;— the number of digits in the number. The second line contains <span class="tex-span"><i>n</i></span> decimal digits without spaces (but possibly with leading zeroes)&nbsp;— the number initially stored in the display computer. The following <span class="tex-span"><i>n</i></span> lines contain 10 characters each. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th of these lines is the code character for a digit <span class="tex-span"><i>j</i> - 1</span> in position <span class="tex-span"><i>i</i></span>, most significant digit positions are described first.</p>

## Output

<p>For each test case print an integer: the number of seconds until Borya definitely knows what was the initial number stored on the display of the computer. Do not print leading zeroes.</p>





```input1
3
2
42
abcdefghij
jihgfedcba
2
42
aaaaaaaaaa
aaaaaaaaaa
1
2
abcdabcdff

```




```output1
0
58
2

```


