## Description

<div><p>Max wants to buy a new skateboard. He has calculated the amount of money that is needed to buy a new skateboard. He left a calculator on the floor and went to ask some money from his parents. Meanwhile his little brother Yusuf came and started to press the keys randomly. Unfortunately Max has forgotten the number which he had calculated. The only thing he knows is that the number is divisible by <span class="tex-span">4</span>.</p><p>You are given a string <span class="tex-span"><i>s</i></span> consisting of digits (the number on the display of the calculator after Yusuf randomly pressed the keys). Your task is to find the number of substrings which are divisible by <span class="tex-span">4</span>. A substring can start with a zero.</p><p>A substring of a string is a nonempty sequence of consecutive characters.</p><p>For example if string <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-tt">124</span> then we have four substrings that are divisible by <span class="tex-span">4</span>: <span class="tex-font-style-tt">12</span>, <span class="tex-font-style-tt">4</span>, <span class="tex-font-style-tt">24</span> and <span class="tex-font-style-tt">124</span>. For the string <span class="tex-font-style-tt">04</span> the answer is three: <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">4</span>, <span class="tex-font-style-tt">04</span>.</p><p>As input/output can reach huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">gets/scanf/printf</span> instead of <span class="tex-font-style-tt">getline/cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>.</p></div><div class="input-specification"><p>The only line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 3·10<sup class="upper-index">5</sup></span>). The string <span class="tex-span"><i>s</i></span> contains only digits from <span class="tex-span">0</span> to <span class="tex-span">9</span>.</p></div><div class="output-specification"><p>Print integer <span class="tex-span"><i>a</i></span> — the number of substrings of the string <span class="tex-span"><i>s</i></span> that are divisible by <span class="tex-span">4</span>.</p><p>Note that the answer can be huge, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p></div>

## Input

<p>The only line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 3·10<sup class="upper-index">5</sup></span>). The string <span class="tex-span"><i>s</i></span> contains only digits from <span class="tex-span">0</span> to <span class="tex-span">9</span>.</p>

## Output

<p>Print integer <span class="tex-span"><i>a</i></span> — the number of substrings of the string <span class="tex-span"><i>s</i></span> that are divisible by <span class="tex-span">4</span>.</p><p>Note that the answer can be huge, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p>





```input1
124

```




```input2
04

```




```input3
5810438174

```




```output1
4

```




```output2
3

```




```output3
9

```


