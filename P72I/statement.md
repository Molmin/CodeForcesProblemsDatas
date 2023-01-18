## Description

<div><p>The non-negative integer <span class="tex-span"><i>a</i></span> is a divisor of the non-negative integer <span class="tex-span"><i>b</i></span> if and only if there exists a <span class="tex-font-style-bf">positive</span> integer <span class="tex-span"><i>c</i></span> such that <span class="tex-span"><i>a</i> × <i>c</i> = <i>b</i></span>. </p><p>Some numbers are really interesting. Commander Surena defines some interesting properties for non-negative integers:</p><ul> <li> An integer is <span class="tex-font-style-underline">happy</span> if it is divisible by at least one of its digits and not by all of them. </li><li> An integer is <span class="tex-font-style-underline">happier</span> if it is divisible by all of its digits. </li><li> An integer is <span class="tex-font-style-underline">upset</span> if it's divisible by none of its digits. </li></ul><p>Surena asks you to find out if a given number is happy, happier or upset.</p></div><div class="input-specification"><p>Input contains a single non-negative integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>).</p></div><div class="output-specification"><p>Write on a single line the type of the integer: <span class="tex-font-style-tt">happy</span>, <span class="tex-font-style-tt">happier</span> or <span class="tex-font-style-tt">upset</span>. Print the type in lowercase letters.</p></div>

## Input

<p>Input contains a single non-negative integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>).</p>

## Output

<p>Write on a single line the type of the integer: <span class="tex-font-style-tt">happy</span>, <span class="tex-font-style-tt">happier</span> or <span class="tex-font-style-tt">upset</span>. Print the type in lowercase letters.</p>





```input1
99

```




```input2
29994

```




```input3
23

```




```output1
happier

```




```output2
happy

```




```output3
upset

```



## Note

<p>In the second test <span class="tex-span">29994</span> is only divisible by <span class="tex-span">2</span>.</p><p>In the third test <span class="tex-span">23</span> is a prime number.</p>
