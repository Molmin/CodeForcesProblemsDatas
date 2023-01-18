## Description

<div><p>Karen is getting ready for a new school day!</p><center> <img class="tex-graphics" src="file://rjQX9Vc1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It is currently <span class="tex-font-style-tt">hh:mm</span>, given in a 24-hour format. As you know, Karen loves <span class="tex-font-style-it">palindromes</span>, and she believes that it is good luck to wake up when the time is a palindrome.</p><p>What is the minimum number of minutes she should sleep, such that, when she wakes up, the time is a palindrome?</p><p>Remember that a palindrome is a string that reads the same forwards and backwards. For instance, <span class="tex-font-style-tt">05:39</span> is not a palindrome, because <span class="tex-font-style-tt">05:39</span> backwards is <span class="tex-font-style-tt">93:50</span>. On the other hand, <span class="tex-font-style-tt">05:50</span> is a palindrome, because <span class="tex-font-style-tt">05:50</span> backwards is <span class="tex-font-style-tt">05:50</span>.</p></div><div class="input-specification"><p>The first and only line of input contains a single string in the format <span class="tex-font-style-tt">hh:mm</span> (<span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">hh</span> <span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">mm</span> <span class="tex-span"> ≤ 59</span>).</p></div><div class="output-specification"><p>Output a single integer on a line by itself, the minimum number of minutes she should sleep, such that, when she wakes up, the time is a palindrome.</p></div>

## Input

<p>The first and only line of input contains a single string in the format <span class="tex-font-style-tt">hh:mm</span> (<span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">hh</span> <span class="tex-span"> ≤ 23</span>, <span class="tex-span">00 ≤ </span> <span class="tex-font-style-tt">mm</span> <span class="tex-span"> ≤ 59</span>).</p>

## Output

<p>Output a single integer on a line by itself, the minimum number of minutes she should sleep, such that, when she wakes up, the time is a palindrome.</p>





```input1
05:39

```




```input2
13:31

```




```input3
23:59

```




```output1
11

```




```output2
0

```




```output3
1

```



## Note

<p>In the first test case, the minimum number of minutes Karen should sleep for is <span class="tex-span">11</span>. She can wake up at <span class="tex-font-style-tt">05:50</span>, when the time is a palindrome.</p><p>In the second test case, Karen can wake up immediately, as the current time, <span class="tex-font-style-tt">13:31</span>, is already a palindrome.</p><p>In the third test case, the minimum number of minutes Karen should sleep for is <span class="tex-span">1</span> minute. She can wake up at <span class="tex-font-style-tt">00:00</span>, when the time is a palindrome.</p>
