## Description

<div><p><span class="tex-font-style-it">The problem uses a simplified TCP/IP address model, please read the statement carefully.</span></p><p>An IP address is a 32-bit integer, represented as a group of four decimal 8-bit integers (without leading zeroes), separated by commas. For example, record <span class="tex-font-style-tt">0.255.1.123</span> shows a correct IP address and records <span class="tex-font-style-tt">0.256.1.123</span> and <span class="tex-font-style-tt">0.255.1.01</span> do not. In the given problem an arbitrary group of four 8-bit integers is a correct IP address.</p><p>Our hero Polycarpus still works as a system administrator in some large corporation. He likes beautiful IP addresses. To check if some IP address is beautiful, he should do the following:</p><ol> <li> write out in a line four 8-bit numbers of the IP address, without the commas; </li><li> check if the resulting string is a palindrome. </li></ol><p>Let us remind you that a palindrome is a string that reads the same from right to left and from left to right.</p><p>For example, IP addresses <span class="tex-font-style-tt">12.102.20.121</span> and <span class="tex-font-style-tt">0.3.14.130</span> are beautiful (as strings "<span class="tex-font-style-tt">1210220121</span>" and "<span class="tex-font-style-tt">0314130</span>" are palindromes), and IP addresses <span class="tex-font-style-tt">1.20.20.1</span> and <span class="tex-font-style-tt">100.4.4.1</span> are not.</p><p>Polycarpus wants to find all beautiful IP addresses that have the given set of digits. Each digit from the set must occur in the IP address at least once. IP address must not contain any other digits. Help him to cope with this difficult task.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10)</span> — the number of digits in the set. The second line contains the set of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 9)</span>. It is guaranteed that all digits in the set are distinct.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span> — the number of beautiful IP addresses that contain the given set of digits. In the following <span class="tex-span"><i>k</i></span> lines print the IP addresses, one per line in the arbitrary order.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10)</span> — the number of digits in the set. The second line contains the set of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 9)</span>. It is guaranteed that all digits in the set are distinct.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span> — the number of beautiful IP addresses that contain the given set of digits. In the following <span class="tex-span"><i>k</i></span> lines print the IP addresses, one per line in the arbitrary order.</p>





```input1
6
0 1 2 9 8 7

```




```input2
1
4

```




```output1
6
78.190.209.187
79.180.208.197
87.190.209.178
89.170.207.198
97.180.208.179
98.170.207.189

```




```output2
16
4.4.4.4
4.4.4.44
4.4.44.4
4.4.44.44
4.44.4.4
4.44.4.44
4.44.44.4
4.44.44.44
44.4.4.4
44.4.4.44
44.4.44.4
44.4.44.44
44.44.4.4
44.44.4.44
44.44.44.4
44.44.44.44

```


