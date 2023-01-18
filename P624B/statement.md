## Description

<div><p>You are given an alphabet consisting of <span class="tex-span"><i>n</i></span> letters, your task is to make a string of the maximum possible length so that the following conditions are satisfied: </p><ul> <li> the <span class="tex-span"><i>i</i></span>-th letter occurs in the string no more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> times; </li><li> the number of occurrences of each letter in the string must be <span class="tex-font-style-bf">distinct</span> for all the letters that occurred in the string at least once. </li></ul></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤  26</span>)&nbsp;— the number of letters in the alphabet.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— <span class="tex-span"><i>i</i></span>-th of these integers gives the limitation on the number of occurrences of the <span class="tex-span"><i>i</i></span>-th character in the string.</p></div><div class="output-specification"><p>Print a single integer — the maximum length of the string that meets all the requirements.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤  26</span>)&nbsp;— the number of letters in the alphabet.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— <span class="tex-span"><i>i</i></span>-th of these integers gives the limitation on the number of occurrences of the <span class="tex-span"><i>i</i></span>-th character in the string.</p>

## Output

<p>Print a single integer — the maximum length of the string that meets all the requirements.</p>





```input1
3
2 5 5

```




```input2
3
1 1 2

```




```output1
11

```




```output2
3

```



## Note

<p>For convenience let's consider an alphabet consisting of three letters: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>". In the first sample, some of the optimal strings are: "<span class="tex-font-style-tt">cccaabbccbb</span>", "<span class="tex-font-style-tt">aabcbcbcbcb</span>". In the second sample some of the optimal strings are: "<span class="tex-font-style-tt">acc</span>", "<span class="tex-font-style-tt">cbc</span>".</p>
