## Description

<div><p>You are given a binary string <span class="tex-span"><i>s</i></span> (each character of this string is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>).</p><p>Let's denote the cost of string <span class="tex-span"><i>t</i></span> as the number of occurences of <span class="tex-span"><i>s</i></span> in <span class="tex-span"><i>t</i></span>. For example, if <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-tt">11</span> and <span class="tex-span"><i>t</i></span> is <span class="tex-font-style-tt">111011</span>, then the cost of <span class="tex-span"><i>t</i></span> is <span class="tex-span">3</span>.</p><p>Let's also denote the Fibonacci strings sequence as follows:</p><ul><li> <span class="tex-span"><i>F</i>(0)</span> is <span class="tex-font-style-tt">0</span>;</li><li> <span class="tex-span"><i>F</i>(1)</span> is <span class="tex-font-style-tt">1</span>;</li><li> <span class="tex-span"><i>F</i>(<i>i</i>) = <i>F</i>(<i>i</i> - 1) + <i>F</i>(<i>i</i> - 2)</span> if <span class="tex-span"><i>i</i> &gt; 1</span>, where <span class="tex-span"> + </span> means the concatenation of two strings.</li></ul><p>Your task is to calculate the sum of costs of all subsequences of the string <span class="tex-span"><i>F</i>(<i>x</i>)</span>. Since answer may be large, calculate it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 100</span>) — the length of <span class="tex-span"><i>s</i></span> and the index of a Fibonacci string you are interested in, respectively.</p><p>The second line contains <span class="tex-span"><i>s</i></span> — a string consisting of <span class="tex-span"><i>n</i></span> characters. Each of these characters is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>Print the only integer — the sum of costs of all subsequences of the string <span class="tex-span"><i>F</i>(<i>x</i>)</span>, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 100</span>) — the length of <span class="tex-span"><i>s</i></span> and the index of a Fibonacci string you are interested in, respectively.</p><p>The second line contains <span class="tex-span"><i>s</i></span> — a string consisting of <span class="tex-span"><i>n</i></span> characters. Each of these characters is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>Print the only integer — the sum of costs of all subsequences of the string <span class="tex-span"><i>F</i>(<i>x</i>)</span>, taken modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p>





```input1
2 4
11

```




```input2
10 100
1010101010

```




```output1
14

```




```output2
553403224

```


