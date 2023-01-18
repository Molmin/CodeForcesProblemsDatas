## Description

<div><p>You know that the Martians use a number system with base <span class="tex-span"><i>k</i></span>. Digit <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>b</i> &lt; <i>k</i></span>) is considered <span class="tex-font-style-it">lucky</span>, as the first contact between the Martians and the Earthlings occurred in year <span class="tex-span"><i>b</i></span> (by Martian chronology).</p><p>A <span class="tex-font-style-it">digital root</span> <span class="tex-span"><i>d</i>(<i>x</i>)</span> of number <span class="tex-span"><i>x</i></span> is a number that consists of a single digit, resulting after cascading summing of all digits of number <span class="tex-span"><i>x</i></span>. Word "cascading" means that if the first summing gives us a number that consists of several digits, then we sum up all digits again, and again, until we get a one digit number.</p><p>For example, <span class="tex-span"><i>d</i>(3504<sub class="lower-index">7</sub>) = <i>d</i>((3 + 5 + 0 + 4)<sub class="lower-index">7</sub>) = <i>d</i>(15<sub class="lower-index">7</sub>) = <i>d</i>((1 + 5)<sub class="lower-index">7</sub>) = <i>d</i>(6<sub class="lower-index">7</sub>) = 6<sub class="lower-index">7</sub></span>. In this sample the calculations are performed in the 7-base notation.</p><p>If a number's digital root equals <span class="tex-span"><i>b</i></span>, the Martians also call this number lucky.</p><p>You have string <span class="tex-span"><i>s</i></span>, which consists of <span class="tex-span"><i>n</i></span> digits in the <span class="tex-span"><i>k</i></span>-base notation system. Your task is to find, how many distinct substrings of the given string are lucky numbers. Leading zeroes are permitted in the numbers.</p><p>Note that substring <span class="tex-span"><i>s</i>[<i>i</i>... <i>j</i>]</span> of the string <span class="tex-span"><i>s</i> = <i>a</i><sub class="lower-index">1</sub><i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>) is the string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>a</i><sub class="lower-index"><i>i</i> + 1</sub>... <i>a</i><sub class="lower-index"><i>j</i></sub></span>. Two substrings <span class="tex-span"><i>s</i>[<i>i</i><sub class="lower-index">1</sub>... <i>j</i><sub class="lower-index">1</sub>]</span> and <span class="tex-span"><i>s</i>[<i>i</i><sub class="lower-index">2</sub>... <i>j</i><sub class="lower-index">2</sub>]</span> of the string <span class="tex-span"><i>s</i></span> are different if either <span class="tex-span"><i>i</i><sub class="lower-index">1</sub> ≠ <i>i</i><sub class="lower-index">2</sub></span> or <span class="tex-span"><i>j</i><sub class="lower-index">1</sub> ≠ <i>j</i><sub class="lower-index">2</sub></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>b</i> &lt; <i>k</i></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains string <span class="tex-span"><i>s</i></span> as a sequence of <span class="tex-span"><i>n</i></span> integers, representing digits in the <span class="tex-span"><i>k</i></span>-base notation: the <span class="tex-span"><i>i</i></span>-th integer equals <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>k</i></span>) — the <span class="tex-span"><i>i</i></span>-th digit of string <span class="tex-span"><i>s</i></span>. The numbers in the lines are space-separated.</p></div><div class="output-specification"><p>Print a single integer — the number of substrings that are lucky numbers.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specifier.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>b</i> &lt; <i>k</i></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains string <span class="tex-span"><i>s</i></span> as a sequence of <span class="tex-span"><i>n</i></span> integers, representing digits in the <span class="tex-span"><i>k</i></span>-base notation: the <span class="tex-span"><i>i</i></span>-th integer equals <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>k</i></span>) — the <span class="tex-span"><i>i</i></span>-th digit of string <span class="tex-span"><i>s</i></span>. The numbers in the lines are space-separated.</p>

## Output

<p>Print a single integer — the number of substrings that are lucky numbers.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specifier.</p>





```input1
10 5 6
3 2 0 5 6 1

```




```input2
7 6 4
3 5 0 4

```




```input3
257 0 3
0 0 256

```




```output1
5
```




```output2
1
```




```output3
3
```



## Note

<p>In the first sample the following substrings have the sought digital root: <span class="tex-span"><i>s</i>[1... 2]</span> = "3 2", <span class="tex-span"><i>s</i>[1... 3]</span> = "3 2 0", <span class="tex-span"><i>s</i>[3... 4]</span> = "0 5", <span class="tex-span"><i>s</i>[4... 4]</span> = "5" and <span class="tex-span"><i>s</i>[2... 6]</span> = "2 0 5 6 1".</p>
